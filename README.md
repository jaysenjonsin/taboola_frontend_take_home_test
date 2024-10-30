Code explained:
Once running the code, the output of the first part will be readable in the console as a console.log as a JSON.stringified object containing the top 25 most common words, including how many time each word is included in the web page. Within the code is the definition of the replaceCommonText function. The replaceCommonText function will be runnable in the console by calling the replaceCommonText function with an argument of a string. If an argument isn't provided to replaceCommonText, it will run with the document.body.innerText as the argument. The return will be in the console.

resources used:
-Figuring out how to grab text from a web page: https://stackoverflow.com/questions/13205289/javascript-how-to-retrieve-text-from-a-webpage

-Writing regex to filter out punctuation, numbers, symbols in the getCommonWords function: ChatGPT

-writing regex to identify words in a string: ChatGPT

-looking up how to define a function that can be used in the console after execution of the main function (utilizing window.replaceCommonText rather than just defining replaceCommonText as a function): ChatGPT

-creating array consisting of key and value from an object: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object/entries

-converting array of arrays consisting of key and value pairs back into an object: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object/fromEntries

Other thoughts:

- Definitely possible to create a solution for splitting words on spaces and filtering without the use of regex, but opted to use regex for better time complexity and cleaner implementation.
- Initially returned top words as a sorted array for first part, decided to convert back to an object before replacing the text as it is easier to implement in the replaceCommonText function for the second part
  -considered third party libraries: axios for data fetching
