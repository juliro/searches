# searches
google search
$ npm install google-search-scraper
var scraper = require('google-search-scraper');

var options = {
  query: 'austrian schools violence',
  limit: 20
};

scraper.search(options, function(err, url) {
  // This is called for each result
  if(err) throw err;
  console.log(url)
});
