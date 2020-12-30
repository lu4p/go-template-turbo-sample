# go-template-turbo-sample
This is a sample project to show how to use Go (templates) with Turbo.

This project uses:
- [Go](https://golang.org/), a programming language that makes it easy to build simple, reliable, and efficient software.
- [html/template](https://pkg.go.dev/html/template), a html templating library included in the stdlib of Go
- [Echo](https://echo.labstack.com/), a Go web framework
- [Turbo](https://turbo.hotwire.dev/), part of [Hotwire](https://hotwire.dev/) a new approach from Basecamp for writing modern web applications without much JavaScript
- [tailwindcss](https://tailwindcss.com/), makes HTML look nice
- [webpack](https://webpack.js.org/), for packing JS and CSS into single files, with minimization enabled, setup to extract CSS to a seperate file 
- [Air](https://github.com/cosmtrek/air), for hot reloading Go code and templates on change.
- some `npm run` commands

- [Echo](https://echo.labstack.com/), a web framework for Go
- [Turbo](https://turbo.hotwire.dev/), brings in the speed of a single-page web application without writing any JavaScript
- [tailwindcss](https://tailwindcss.com/), makes things look nice, complete setup with purging of unused css, postcss and autoprefixer
- [webpack](https://webpack.js.org/), for packing JS and CSS into single files, with minimization enabled, setup to extract CSS to a seperate file 
- [Air](https://github.com/cosmtrek/air), for hot reloading Go code and templates on change.

## Setup
You need to have [go](https://golang.org/dl/) and [npm](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm) installed.

```sh
go get -u github.com/cosmtrek/air
git clone https://github.com/lu4p/go-template-turbo-sample.git
cd templates-turbo-sample
npm install
npm run dev
```

After all of this just run `air`, to start the webapp and enable hot reload.

The `dist/main.css` file is rather large now at ~6MB, but don't worry this is only becasue each possible class of tailwind is included (there a many), once you build for production only ~4KB of CSS is left.

If you want to also rebuild the JS and CSS on change run `npm run watch` in a seperate terminal session.

To build for production run `npm run prod` and `go build`.
