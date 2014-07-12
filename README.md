# adorable-avatars

## What are avatars?
Avatars are earthly creatures that serve as proxies for gods.
In the web world, they just represent people, and they're usually small images. 

Some use photographs of themselves as their avatar. Some people use caricatures of themselves. Others pick their favorite superhero. The sky's the limit.

## What's an avatar _service_?
It answers the question "What is this user's avatar?"
In this way, it provides a consistent representation of that user.
Across _all_ websites that use that service. Pretty cool, right?

But what if you haven't uploaded your image to that service?
Then you get a really boring, gray silhouette.

## So what's the Adorable Avatar service?
It's an interface to a better universe. With a simple route, your face will be filled with consistently-linked avatar glory!

_Consistently-linked avatar glory_ What?

Whenever you make a request to Adorable Avatars, using an identifier like "abott@adorable.io," we give you an image for you to use on your page.
Most importantly, it's the same image! Every. Single. Time.

## Why would I use it?
What if you're developing a feature like member lists or profiles, but you don't have any images to use?
Just give us your user's identifier and we'll give you their avatar image!
That's it.

Already have avatars implemented in your application?
Use Adorable Avatars as a fallback and get rid of those gray silhouettes!

## How do I use it?
1. Clone this repo
2. Install dependencies: `npm install`
3. Start the server: `npm start`

### Requesting an Avatar
The most basic request is of the following form:

    http://localhost:3002/avatar/<identifier>

Where `identifier` is the unique identifier for your user (name, email, md5, etc.).
This will serve the image in its default size.

To request an avatar with specific dimensions, use the following form:

    http://localhost:3002/avatar/<dimensions>/<identifier>

Where `dimensions` specifies the width and height, e.g. "300x300" or "400x200."

So, if you want your friend Bob's avatar, with a width of 640px and a height of 480px, the URL would be:

    http://localhost:3002/avatar/640x480/bob
