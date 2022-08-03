---
id: 23ulirxpybd19oza5yzzfiw
title: Managing Contacts
desc: How to use Dendron to keep track of your contacts
updated: 1659494972076
created: 1659483615000
---

{{fm.desc}}

This workflow covers:
- keeping a note on each person
- keeping track of messages

## Files
- schema: user schema [^1]
- traits: `msg` trait[^3]
- templates
	- [[template.user]]: template used for users
	- [[template.msg]]: template used for messages

## Getting Started

### Create a new user

To create a new user, open lookup and create a new person under the `user` hierarchy (eg. `user.john`)

<div style="position: relative; padding-bottom: 64.5933014354067%; height: 0;"><iframe src="https://www.loom.com/embed/2b4532c852154b49b246cd887c3ec3f2" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;"></iframe></div>

> NOTE: notice that this note is created with frontmatter - this is because of the user schema [^1] file which automatically applies thte user template[^2]  YOu can customize this template based on your specific needs

### Add a new message

To record (or author) a message with the user, use the message note trait[^3] to createa new message

1. Go to a user note (eg. [[user.jonny-seed]])
1. Run [[Create Note with Trait|dendron.topic.traits.commands.create-note-with-trait]] and select `msg`
1. Add a human readable suffix at the end of the generated message hierarchy (eg. `user.jonny-seed.msg.2022.08.02.catchup`)

<div style="position: relative; padding-bottom: 64.5933014354067%; height: 0;"><iframe src="https://www.loom.com/embed/05c10f2d3cd34a68a50ea4c8c9206373" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;"></iframe></div>


[^1]: [[notes/user.schema.yml]]: user schema file
[^2]: [[template.user]]: template used for given user
[^3]: [[noteTraits/msg.js]]: custom message note trait