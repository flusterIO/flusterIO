# FlusterIO

![Fluster banner](fluster_banner.png)

> Beginning of a docs rewrite for the upcoming release of the Apple specific applications, so some of these docs refer to new features. Both applications are pretty much complete, but I'm homeless... so I'm struggling to afford that fx$\*@ng Apple developer license.

To make a long story short, Fluster is a new rendition of an application that I built for [my own academic pursuits](https://www.flusterapp.com/docs/my_work/on_the_gravitational_nature_of_time). The search & linking features helped me organize my thoughts better than any application available, and I hope they'll help you organize your thoughts too.

Here's a few of the features on initial release:

- [x] Full, multi-page free-draw canvas
- [x] Integrated Mdx editor with:
  - [x] Component Snippets
  - [x] Syntax Highlighting
  - [x] Vim support
  - [x] Emacs support
- [x] Searchability features:
  - [x] Search by tag
  - [x] Search by topic
  - [x] Search by subject
  - [x] Search by citation
  - [x] Full-text search with syntax specific re-ranking for improved search accuracy
  - [ ] Semantic search
    - This was included on-device in the Tauri based version of Fluster. It's unlikely that a _completely_ on device vector store will make it's way back to Fluster, but a future version will include support for an off-device vector store as a paid service.
- [x] Integrated bibliography manager with csl support. Current release only supports using embedded csl files, narrowing the options down to about 20, but future versions will allow providing your own csl file.

## Future Plans

Future plans are to become a more Jupyter-friendly note taking framework that's capable of meeting the needs of the most advanced academics, but simple enough for everyone. The plan is to build a python-esk domain specific language for note related tasks like math calculations, generating plots, and even interacting with the file system on desktop... directly from within your note, and then move to a Swift-first rendering layout where mdx is rendered in a 'cell' of a native layout, rather than in completely separate component. This would allow writing mobile-friendly, high-performant Jupyter compatible notebooks in a markdown-first syntax, but this is a big undertaking. If this interests you, please consider supporting the application. A previous version of this app is what helped me, and I hope a future version of this app can help many people.
