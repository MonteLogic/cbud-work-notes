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


Side note: Dilemma: 

If we want to ship fast we will skip features which enhance UI but if we commit and get onto the next part, the features we skipped which will be added on later will be much tougher to add on due to the fact that we have to re-establish the app in that 'mindspace' and 'codespace' to create said feature.



...

We also have the problem of, they already might be an a functional org but they choose to make a new one anyway. So there should be an org switch as one of the options on an empty 'main/schedule'. 



### ... 

Now we got a good way of getting a new user on, now we have to get the Lorem Ipsum route working.

I don't even know how the route management even works.

I think it's copied in from Clerk and they are duplicated, but I think this is whack. 

The Clerk org should hold the metadata so, there's not an issue of duplication but this will throw off the rest of the app.


// Make GH issue hotkey for vim. So you can use a : and then an issue template will be written.

### ...

We just have to inject the lorem Ipsum template on creation.

### We are trying to create a sample route on org creation



