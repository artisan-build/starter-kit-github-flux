# Verbs-Driven Livewire Starter Kit for GitHub-Exclusive Authentication

By [Ed Grosvenor](https://github.com/edgrosvenor), Co-Founder / CEO at [Artisan Build, Inc](https://artisan.build)

This starter kit is for applications that exclusively use GitHub for user creation and authentication. A simple example
of this is the [Artisan Build Community](https://artisan.community). It is a good option for developer tools in an 
ecosystem where you know that all of your users will have GitHub accounts, particularly if you need access to their
GitHub accounts to provide services anyway.


![Image](https://github.com/user-attachments/assets/16880b0d-44be-4c67-a1cd-bc3a6b4a1158)

### Why Did I Build This Starter Kit?

This starter kit doesn't offer anything that isn't possible using Laravel's first-party WorkOS integration except for
the [Verbs](https://verbs.thunk.dev/) integration. The way the WorkOS integration is written, it isn't possible to fire
a Verbs event when a user is created. 

### A Note About Verbs

This starter kit currently uses `dev-main` for Verbs because Verbs has not yet hit 1.0 and the currently tagged
version contains code that will break when they do tag 1.0. If you need to work with a tagged version, you can 
update the dependency to the most recent release without any problem. None of the code that is due to break (singleton 
states) is used in this starter kit itself. I do, however, use them extensively in the applications I build using this
starter kit, so I've pegged the start kit to `dev-main` for my own convenience. If you are planning to go all-in on
Verbs like we have, I recommend that you leave it that way until the 1.0 release.
