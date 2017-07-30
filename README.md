#Node.js | USDA Nutrient Database wrapper
Our functions provides access to the USDA Food Composition Databases. It is intended primarily to assist application developers wishing to incorporate nutrient data into their applications or websites.

This is a Node.js API wrapper for the USDA Nutrient Database REST API.

For brief documentation please visit -- <a href="https://ndb.nal.usda.gov/ndb/doc/">USDA Food Composition Databases</a>
# Installation

Install via NPM

```js

npm install nutrient-database --save

```

# Example

i. FoodReport

```js

var ndb = require('nutrient-database');

// Parameters:
// 1. ndb no
// 2. API Key
ndb.foodReport('01009','DEMO_KEY', function(err, response){
    console.log(JSON.stringify(response));
});

```

ii. List

```js

var ndb = require('nutrient-database');

// Parameters:
// 1. List Type
// 2. Maximum number
// 3. Offset
// 4. API Key
ndb.list('f','','','DEMO_KEY', function(err, response){
    console.log(JSON.stringify(response));
});

```

iii. Search

```js

var ndb = require('nutrient-database');

// Parameters:
// 1. Search Query
// 2. Dataset
// 3. Maximum number
// 4. Offset
// 5. API Key
ndb.search('cheese','','','','DEMO_KEY', function(err, response){
    console.log(JSON.stringify(response));
});

```

# Any issue or want more features? Contact me!

This module has been tested under limited scenarios. If you find any issue please feel free to report via one of the below platforms:

Github: <a href="https://github.com/harshdoshi999/nutrient-database/issues">nutrient-database</a> | 
Email: harshdoshi999@gmail.com | 
Skype: harshxxx3
