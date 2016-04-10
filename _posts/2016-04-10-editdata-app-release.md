---
title: "New release of app.editdata.org"
layout: page
published: true
author: Seth Vincent
---

Over the past few months we've been working on a new release of the [EditData app](http://app.editdata.org). Here's a roundup of where things are at.

## What's new

### Flatsheet is now EditData

We've been slowly renaming things from Flatsheet to EditData. The goal is to take focus away from spreadsheets and make the project about data editing & workflow using whatever method is most effective. Plus now the project doesn't share a name with a type of bedding.

### Revised domains

The EditData app used to call editdata.org home. The app is now at [app.editdata.org](http://app.editdata.org), and you'll find documentation & the blog at [editdata.org](http://editdata.org).

### Better support for field types other than strings.

In the EditData app you can now have columns that are numbers, images, links, & lists (arrays) in addition to strings. This is still somewhat experimental. Let us know if you experience any issues.

### EditData app is built from reusable components

Previously the UI components in the EditData app couldn't be used separately very easily. Now we have the following modules that can be used on their own:

- [data-grid](https://github.com/editdata/data-grid)
- [data-form](https://github.com/editdata/data-form)
- [data-fields](https://github.com/editdata/data-fields)
- [list-editor](https://github.com/editdata/list-editor)

## What's coming up

### Making pull requests through The EditData app.

We made a demo called [submit-data](https://github.com/editdata/submit-data) that shows how to use JavaScript & the GitHub API to easily perform the following workflow:

- fork a repository
- create a new branch on the fork
- edit a file
- commit the changes
- create a pull request on the original repository

We'll be adding this functionality to app.editdata.org next.

### A JavaScript module that makes it easy to make pull requests

As part of adding pull requests to the EditData app, we're creating a module that anyone can reuse to add similar fork > branch > commit > pull request functionality to their apps. That work is happening in the [editdata-github](https://github.com/editdata/editdata-github) repository.

### Experimenting with modules we're using to create UI components

So far all modules are created using [virtual-dom](https://github.com/matt-esch/virtual-dom). We'll be trying out a few similar modules, particularly [yo-yo.js](https://github.com/maxogden/yo-yo). The focus will be on making EditData UI components as easy to create & maintain as possible.

### Additional field types & improved UI for existing types

Next on the list of field types we'll support is geojson! That will be exciting. We'll also support lists in a key/value format that export as objects.

## Consulting

As an open-source project EditData has previously received grants ([Open News](http://editdata.org/posts/getting-flatsheet-to-v1-with-help-from-opennews), [Knight Prototype Fund](http://editdata.org/posts/flatsheet-supported-by-knight-prototype-fund)) to support the development. We're now taking on consulting projects with clients that want to build similar applications. We can work together to build custom data editing & workflow apps for your organization, & in turn that will support the continued development of the EditData project. Send an email to hi @ editdata.org if you're interested.
