hugo-snippets
=============

Convenient partials, layouts and shortcodes for Hugo (gohugo.io)

## Conventions

### Site Config (TOML)

#### Social Details
	+++
	[params]
	  [params.social]
	    github		= "nozzle"
	    facebook		= "nozzleio"
	    facebook_admin	= "17807199"  # This needs to be a page admin to get domain insights
	    twitter		= "nozzleio"
	    twitter_domain	= "nozzle.io" # This domain shows in twitter cards as "View on `twitter_domain`"
	    googleplus		= "NozzleIo"
	    pinterest		= "nozzleio"
	    instagram		= "nozzleio"
	    youtube		= "nozzleio"
	    linkedin		= "nozzleio"
	+++

#### Author Details
	+++
	[params]
	  [params.authors]
	    [params.authors.John]

	      name			= "John Connor"
	      thumbnail		= "http://std3.ru/90/ff/1369441968-90ff032a2fa5dc21487fb9618977c803.jpeg"
	      images		= [
	      					"http://www.mirf.ru/Articles/29/5857/T2.jpg",
	      					"http://img2.wikia.nocookie.net/__cb20090810001437/terminator/images/d/dc/John_conor_05.jpg",
	      				  ]
	      bio			= "John Connor is the son of Sarah Connor and Kyle Reese, and the leader of the worldwide human resistance..."
	      email			= "johnconner@gmail.com"

	      [params.authors.John.social]
	        github			= killskynet"
	        facebook		= killskynet"
	        twitter			= killskynet"
	        googleplus		= killskynet"
	        pinterest		= killskynet"
	        instagram		= killskynet"
	        youtube			= killskynet"
	        linkedin		= killskynet"

	    [params.authors.Sarah]
	    	...
	+++

### Page Front Matter
	+++
	// This needs to map to one of the authors setup in the .Site.Params
	author		= John

	// An array of urls to any images referenced in the post. The first image in the array will be the default shareable image.
	images		 = [
					"http://www.mirf.ru/Articles/29/5857/T2.jpg",
					"http://img2.wikia.nocookie.net/__cb20090810001437/terminator/images/d/dc/John_conor_05.jpg",
				  ]

	// An array of urls to any videos referenced in the post. The first video in the array will be the default shareable video.
	videos		 = [
					"https://www.youtube.com/watch?v=WeON54DhMW4",
					"https://www.youtube.com/watch?v=dy5oTJajGOk",
				  ]

	// The first 10 will be inserted into the Google "news_keyword" meta tag
	news_keywords = [ "skynet", "terminator", "john connor" ]

