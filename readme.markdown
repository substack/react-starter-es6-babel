# react-starter-babel-es6

bare-bones [react](https://facebook.github.io/react/) starter
using [babelify](https://npmjs.com/package/babelify) for es6 and jsx
under [browserify](http://browserify.org)/[watchify](https://npmjs.com/package/watchify)
with [npm run scripts](http://substack.net/task_automation_with_npm_run)

forked from [react-starter](https://github.com/substack/react-starter)

[view the starter demo](http://substack.neocities.org/react_starter_babel_es6.html)

# quick start

```
$ npm run watch &
$ npm start
```

# commands

* `npm run build` - build for production
* `npm run watch` - automatically recompile during development
* `npm start` - start a static development web server

# starter code

``` js
import React from 'react'

class App extends React.Component {
  constructor () {
    super()
    this.state = { n: 0 }
  }
  render () {
    return <div>
      <h1>clicked {this.state.n} times</h1>
      <button onClick={this.handleClick.bind(this)}>click me!</button>
    </div>
  }
  handleClick () {
    this.setState({ n: this.state.n + 1 })
  }
}
React.render(<App />, document.querySelector('#content'))
```

# contributing

If you like what you see, but want to add something more, fork this repo and add
your additional feature to the name of the fork. Try to be specific with the
name of your fork, listing the technologies used plus what features the fork
adds.

# variations

Check out the [list of forks](https://github.com/substack/react-starter/network/members)
to see how other people have customized this starter repo.
