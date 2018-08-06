## Answers to technical questions

# How long did you spend on the coding test?

Around 8 hours. I had to refresh my React JS knowledge, that took me some time.

# What would you add to your solution if you had more time?

Many things. For example, color the item that is clicked on, so that the user knows the item whose details are displayed below. The detail section should have bold labels probably.

I test the response time of the user interface (the webpage) and it is not slow. The server is pretty fast, and that allows the application to retrieve information from the server as soon as the user hits a key. This makes the app very interactive. But probably, in case the server is slow, some indication that the information is being retrieved would be needed (for example, something saying "getting data...").

Also, the information retrieval from the server might not need to be done as soon as the user hits a key. It can be deferred until some time has elapsed since the last key was pressed. The idea is not to send unnecessary requests to the server. Or maybe, just put a "Search" button.

I did not implemented the "section of related devices by location", because of time, and also because you can already query in an easy manner the devices with a specific location.

I did not find a way to query the "Location Name" in the API, which sounds like it should be a string. I only found the location, which is a number.

Also, I will comment the code.

# What was the most useful feature that was added to the latest version of your chosen language?

I don't know if it was added to the latest version, but as of JavaScript 1.8.5 you can use ```Object.keys(obj)``` to get an Array of the object ```obj``` properties. So, I did not have to use

```
for (var property in object) {
    if (object.hasOwnProperty(property)) {
        // get value and push back pair (key,value) in a list
    }
}
```

which is very verbose.

# How would you track down a performance issue in production? Have you ever had to do this?

I have done it, but in old school way:
1) Analysis of the code (if I have seen it before or the one who did it is available to sit next to me and explain it). Analyze time complexity, memory complexity, I/O bottleneck.
2) In case the problem could not be detected in the previous step, reproducing the issue in a development server with a copy of the data in production.

Nowadays, I will use a profiler, together with the other tecniques I mentioned.

# How would you improve the Knetik APIs that you just used?

I could not find a way to get the remaining pages. For example, 1000 devices are the result of the query without conditions, but only 25 are returned.
A post request will be needed, where current page in a result set will be a state.

# Please describe yourself using JSON

In javascript, perfect. In java or other languages, it is debatable how good it is. In any case, I am more comfortable using JSON than XML.

