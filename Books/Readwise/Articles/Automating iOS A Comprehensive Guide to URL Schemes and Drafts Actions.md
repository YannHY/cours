# Automating iOS: A Comprehensive Guide to URL Schemes and Drafts Actions

![](https://readwise-assets.s3.amazonaws.com/static/images/article3.5c705a01b476.png)

### Metadata

- Author: Alex Guyot
- Full Title: Automating iOS: A Comprehensive Guide to URL Schemes and Drafts Actions
- Category: #articles
- URL: https://www.macstories.net/tutorials/guide-url-scheme-ios-drafts/

### Highlights

- created by Greg Pierce ([View Highlight](https://instapaper.com/read/1032334945/8170829))
- It is very similar to an “if, then” statement in other programming languages ([View Highlight](https://instapaper.com/read/1032334945/8170835))
- For an easy example, we’ll make our new draft simply say “Hello World”. To percent-encode “Hello World”, you only have to change the space to a “%20” ([View Highlight](https://instapaper.com/read/1032334945/8170996))
- Let’s recap what’s happening in this URL. Since iOS recognizes the steps in a URL action in order, as they come, our action in its current form is already doing four things:
  drafts:// tells iOS to open Drafts.
  x-callback-url/ tells Drafts to enable its built in x-callback parameters. (We’ll get to those later.)
  create? Tells Drafts to create a new draft.
  text=Hello%20World tells Drafts to populate that new draft with the words “Hello World”. ([View Highlight](https://instapaper.com/read/1032334945/8171001))
- drafts://x-callback-url/create?text= ([View Highlight](https://instapaper.com/read/1032334945/8171002))
- To do this, we must continue to the next level of the Drafts URL scheme: “&action=” ([View Highlight](https://instapaper.com/read/1032334945/8171080))
- Tweet: username ([View Highlight](https://instapaper.com/read/1032334945/8171081))
- A colon is percent-encoded to “%3A”, and a space is still “%20”. Our final output will be drafts://x-callback-url/create?text=Hello%20World&action=Tweet%3A%20the_axx. For you, of course, “the_axx” will be whatever your own Twitter username is. ([View Highlight](https://instapaper.com/read/1032334945/8171087))
- There are four x-callback parameters: x-source, x-success, x-error and x-cancel. Here I will only touch on x-success, and a little bit on x-cancel. You can read about the other two at the x-callback-url website. ([View Highlight](https://instapaper.com/read/1032334945/8171092))
- Adding the x-success parameter into your Drafts URL action tells Drafts to perform the next action upon the success of the first one ([View Highlight](https://instapaper.com/read/1032334945/8171097))
- drafts://x-callback-url/create?text=Hello%20World&action=Tweet%3A%20the_axx&x-success= ([View Highlight](https://instapaper.com/read/1032334945/8171101))
- drafts:// tells iOS to open Drafts.
  x-callback-url/ tells Drafts to enable its built in x-callback parameters. (We’ll get to those later.)
  create? Tells Drafts to create a new draft.
  text=Hello%20World tells Drafts to populate that new draft with the words “Hello World”.
  &action="Tweet%3A%20the_axx runs the built-in “Tweet: the_axx” action and posts “Hello World” to my Twitter account.
  &x-success= tells Drafts that once it successfully tweets “Hello World”, it will then perform another action. ([View Highlight](https://instapaper.com/read/1032334945/8171104))
- Now you have to build your second action. This should be pretty simple, because it is exactly the same as your firs ([View Highlight](https://instapaper.com/read/1032334945/8171115))
- Drafts has a fantastic feature in that any time you want to percent-encode a portion of your action, you can simply surround that portion with {{double curly brackets}} ([View Highlight](https://instapaper.com/read/1032334945/8171116))
- The text you are running your next action on, and action you are specifying to run on it, in the second action in your chain actually have to be double encoded ([View Highlight](https://instapaper.com/read/1032334945/8171190))
- Drafts supports a versatile variety of [[variable tags]]. These tags, words wrapped in [[double brackets]] and placed within your URL actions, draw text from various places within whatever draft you run the action on. Better yet, this text is automatically percent-encoded, without you having to do anything. ([View Highlight](https://instapaper.com/read/1032334945/8172020))
- When chaining two Drafts actions together, don’t forget the [First Action]&x-success={{[Second Action]}} template design ([View Highlight](https://instapaper.com/read/1032334945/8210750))
- iOS apps are sandboxed, meaning they are only allowed to interact with the operating system (and other apps) in very limited ways. One of these ways has always been through URL actions. This is how opening a link in any app can automatically move you over to Safari with the corresponding webpage open, or tapping an address can take you into Maps with a pin on the specified location. Safari and Maps both have URL schemes which support this type of communication. Third-party developers have managed to take advantage of this small opening through which apps can “talk” to each other to make incredible things possible by giving their apps powerful URL Schemes. ([View Highlight](https://instapaper.com/read/1032334945/10103775))
- Without x-callback-url, advanced iOS automation would be impossible. ([View Highlight](https://instapaper.com/read/1032334945/10105385))
- The beginning of any Drafts action you ever build should be drafts://x-callback-url/ ([View Highlight](https://instapaper.com/read/1032334945/10105387))
- [[body]] is replaced, when you run your action, by the contents of everything except the first line of your draft. ([View Highlight](https://instapaper.com/read/1032334945/10141751))
- In fact, there’s no difference between [[line|1]] and [[title]]. ([View Highlight](https://instapaper.com/read/1032334945/10184228))
