# expenseTrackerReact

I made this expense tracker app to help me gain more experience with using Rails 5 and React.

I followed an awesome guide by Fernando Villalobos. He provided a very well written step by step guide to build this app from scratch while providing great explanations for everything.
Src: https://www.airpair.com/reactjs/posts/reactjs-a-guide-for-rails-developers
Fernando's GitHub: https://github.com/fervisa/accounts-react-rails

I used the following to build this app -
* Rails 5
* React
* CoffeeScript
* jQuery
* Bootstrap

Before this tutorial I haven't had any experience with CoffeeScript. I felt like this was a great introduction into a useful JS library.

One thing that wasn't working for me was triggering the event of Update to save a change on an existing entry. Specifically it was lines 21-23 of handleEdit in app>assets>javasripts>record.js.coffee

in the tutorial it was - title: React.findDOMNode(@refs.title).value

Everything worked fine once I changed it to -
title: this.refs.title.value
