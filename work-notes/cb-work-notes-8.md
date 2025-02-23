## Start: Fri Feb 21 2025 11:48:58 CST

Feature board

It should be a graph (nodes) of how everything works when it was tested last. Almost like a suite for current features, a switchboard if you will.
Code Switchboard

Not seeing an off the shelf solution for this probably going to have to create a custom solution for this.

...

Local solution which will rely on GH Issues for marking and managing issues.

You could just run 'pnpm start switchboard'
Focusing on Issue 200

This message:

"You are not a part of an organization, Create Organization"

Rather it should always show the slider.

"Ideally you could press a button on the node graph and it starts up the app in THAT state."

Page app/main/schedule/page.tsx

...

Solution:

You are not a part of an organization, start CBud, or get invited to an organization.

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
