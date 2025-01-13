# Schemas
Public schemas for encoding/decoding of binary data. This repo will serve as the publicly accessible repository for all data schemas.

## License
All schemas are fully open source, under the MIT license, usable for personal and commercial purposes. No attribution is implicitely required, no royalties may be imposed, etc. All efforts by anyone involved, present and future, will shouldered by the contributor, all responsibility is indemnified. In layman's terms', "use at your own risk".

## Usage
Simply download and use schemas defined here in your own software, or, if it behooves you and your build process supports it, link directly to the repository files for direct import and compile.

## Definitional
Q: Is this meant to be "authoratative"?
A: Quick answer, of course not. Long answer, yes. If a schema is imported and used in a personal or commercial project, it should be assumed, in so long as Github is generally available, then it should be assumed to be available for import/compilation/usage/etc. In the unlinkely event Github discontinues or discontinues access to public schemas, OpenDataFormats will make any and every possible effort to continue access.

## Structure
Let's say, for example, you want to define a protocol buffer with the following namespace `pub.odf.common.v1.Location`. You would create a pull request for the creation of a file at the namespace of `github.com/odf.pub/schemas/pub.odf.common.v1.Location.proto`. Notice the reverse domain resolution of the file/package's location, based on your organization's URL pattern. It does not have to literally match anything else internally, only be "authoratative" in that it makes sense, and, gives attribution to the potential "owner". OpenDataFormats is always open to new and inventive ways to represent data.

## Backwards Compatibility
The goal is to always support backwards <-> forwards compatibity. Hence the preference for Schema Definition languages, ie; Protocol Buffers, JSON, etc. For example, should you release a new version of your application, say v4, but, you have API servers still serving v3 responses, the latest application should be able to handle older API responses. Conversely, your application is still running v3, but your API is serving v4 responses, neither should introduce 'breaking changes'. Towards this end, we're adhering to Uber's policy of 'namespacing' schemas by their "version" with the `.vX.` naming. Ideally not, but vX to vX+1 should not be "breaking".

We will attempt every effort to not allow for "in major version changes" to be breaking.

## Contributions
Always and extremely welcome! Very simple. Fork the repo, create your additions/updates, send for review, get reviews, update/revise as neccesary, commit and merge, and it will be deployed for general/global use.

## Conflicts
If you believe there are conflicts in this strategy, "Good"! We all want to hear any and every one. The best way is to file a ticket to the issue. It will live "ad infinitum" in Github, for present and future reference. For comparison, see Bitcoin's BIP system, so clean, so traceable, so accountable. We strive for the same. If you have an alternative, please, propose it. Keep in mind a 10+ year time frame. So, don't suggest a link to an ephemeral social media link that also requires a "walled garden" login. We adhere to OG internet principles of openess, the way the internet was originally meant to be built!

## Complaints
See above
