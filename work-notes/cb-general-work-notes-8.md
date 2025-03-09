## Start: Fri Feb 21 2025 11:48:58 CST

Feature board

This message:

"You are not a part of an organization, Create Organization"

Rather it should always show the slider.
Page app/main/schedule/page.tsx

...

Solution:

You are not a part of an organization, start CBud, or request invitation from another group, to an organization.

There should be a counter, if within 10 seconds, they don't click request then go onto create organization.

So it should be:

Start CBud, or request invitation.

And if they start CBud then it should have all the stuff auto-filled and then they can just mindlessly click thru the prompts until they get the schedule view.

## The filled in information

Ideally we could just fill it in automatically and import the component and customize it how we like.

It looks like Clerk already did some of the work seen [here](https://clerk.com/docs/custom-flows/create-organizations).

## This only show if the user has NO org.

http://localhost:3000/main/create-org

## Employees input for Clerk.

Also, there should be an amount of employees input box.

## Start: Sun Feb 23 2025 10:01:19 CST

### Working on issue200

Fresh install should be usable from the start #200

### ...

The org switcher only seems to show the org switcher when there's no payment.

When it switches it stays with the paid one.

### ...

Why the sign-in url:
href={process.env.NEXT_PUBLIC_CLERK_SIGN_IN_URL ?? '/sign-in'}

We also have the problem of, they already might be an a functional org but they choose to make a new one anyway. So there should be an org switch as one of the options on an empty 'main/schedule'.

## Start: Sun Mar 02 2025 10:26:47 CST

Running ads on CBud today.

I swear, I forget, so much stuff, maybe cause I'm getting dumber or whatever, but if we could have a better visual manager for all this work, it would go down way smoother.

Okay, so I ran some ads, on Facebook, which are ads meant to get leads, I'm going to wait for those leads and while I do that I'm going to work on codeboard.js.

## Start: `Sun Mar 09 2025 12:27:51 CDT

Okay,

I am going to do some more finishing touches on CBud the app and then write a bunch of blog posts and then I need to fix the WA so it's actually a good blog and people want to stay on there and read a while.

And what I REALLY want to work on is this Software Management tool which is 3D

There probably already is a WebGL implementation of this.


....
When I'm on a certain menu item, I want that item to be highlighted.

The background color on the home landing page looks 'mad smooth' would like this color scheme for the blog as well. 


