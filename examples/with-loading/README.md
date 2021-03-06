# Example app with page loading indicator

## How to use

Download the example (or clone the repo)[https://github.com/zeit/next.js.git]:

```bash
curl https://codeload.github.com/zeit/next.js/tar.gz/master | tar -xz --strip=2 next.js-master/examples/with-loading
cd with-loading
```

Install it and run:

```bash
npm install
npm run dev
```

Deploy it to the cloud with [now](https://zeit.co/now) ([download](https://zeit.co/download))

```bash
now
```

## The idea behind the example

Sometimes when switching between pages, Next.js needs to download pages(chunks) from the server before rendering the page. And it may also need to wait for the data. So while doing these tasks, browser might be non responsive.

We can simply fix this issue by showing a loading indicator. That's what this examples shows.

It features:

* An app with two pages which uses a common [Header](./components/Header.js) component for navigation links.
* Using `next/router` to identify different router events
* Uses [nprogress](https://github.com/rstacruz/nprogress) as the loading indicator.
