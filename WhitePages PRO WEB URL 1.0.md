# WhitePages PRO Web URL Documentation

*Documentation for WhitePages PRO Web Hyperlink URLs 1.0*

Copyright 2013, WhitePages, Inc.

Last updated: May 6, 2013

## Introduction and Overview

WhitePages PRO Web can simply be integrated with a variety of systems using its simple URL syntax. This syntax allows companies integrating with WhitePages PRO to easily automate the copy and paste performed by their employees, saving significant time and effort for employees who regularly source data in one application and perform investigation using WhitePages PRO.

## URLs 

The WhitePages PRO application is able to perform five basic lookups at the user's request. The URLs accept the identical parameters to the input forms already provided in PRO Web, except those parameters are required to be [URL Encoded](https://en.wikipedia.org/wiki/Percent-encoding) to allow the hyperlink to be correctly parsed by the web browser. There are functions in most major programming languages to [URL Encode](https://en.wikipedia.org/wiki/Percent-encoding) strings.

### Reverse Phone

    https://pro.lookup.whitepages.com/phones?number=<number>
	
The reverse phone parameter takes one parameter - the 10 digit telephone number that is to be looked up.

#### Example

    https://pro.lookup.whitepages.com/phones?number=2069735100
	    

### Reverse Address

    https://pro.lookup.whitepages.com/addresses?street=<street>&where=<region>
	
Reverse address requires two parameters - one which represents the street address, and the other which represents the region, which can be a city, state and/or zip code.

#### Example

    https://pro.lookup.whitepages.com/addresses?street=1301%205th%ave&where=seattle%20wa
    https://pro.lookup.whitepages.com/addresses?street=1301%205th%ave&where=98101


### Find Person

    https://pro.lookup.whitepages.com/people?first_name=<name>&last_name=<last>&where=<region>
	
Find person requires a first name, last name and a region parameter, which can be city, state and/or zip code.

#### Example

    https://pro.lookup.whitepages.com/people?first_name=michael&last_name=mcginn&where=seattle%2C+wa
    https://pro.lookup.whitepages.com/people?first_name=michael&last_name=mcginn&where=98103

### Find Business
    
	https://pro.lookup.whitepages.com/businesses?keywords=<keywords>&where=<region>

Find business searches require business names or keywords in the keywords section, and a location consisting of city, state and/or zip code.

#### Example
    
	https://pro.lookup.whitepages.com/businesses?keywords=starbucks&where=seattle%20wa

## Authentication

If a user is already authenticated, either by checking the "remember me" checkbox, or by having a recent session, links to their browser will immediately request and load the PRO Web results in the browser.

If the user is not logged in, they may log in after the link is clicked. Once they have logged in, they will proceed to the search result page as expected.

Copyright 2013, WhitePages, Inc
