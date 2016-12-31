# Quotation Explorer  :earth_americas: :speech_balloon:

> Explore over 200,000 quotes, with the click of a mouse :earth_americas::speech_balloon:

I wanted to write an web app using only the Golang standard library for routing. I also wanted a simple web API for getting a random quote as JSON.

This app fulfills both my goals: it is [a web app that uses the stdlib for routing, that allows you to click on a single word to quickly and easily
explore quotations](https://quotes.schollz.com) as well as [a way to get quotation JSONs with GET requests](https://quotes.schollz.com/random/3.json). 

## Installation

```
git clone https://github.com/schollz/quotation-explorer.git
cd quotation-explorer
tar -xvzf quotations.db.tar.gz
go get github.com/boltdb/bolt/...
go get gopkg.in/cheggaaa/pb.v1
go build
./quotation-explorer
```

## Usage

Open a web browser and explore quotations!

## More information

The quotations are stoed in the BoltDB `quotations.db` which is archived in the repo. The quotations are stored in a bucket `data` and indexed in a bucket `index`. 

## License

MIT