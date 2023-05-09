Hi! I'm Tom.

I've been doing full-stack web development and Linux[^1] system
administration for a *long* time — since I was a teenager in the 1990s.
I somehow ended up [co-founding and successfully selling a
company][ign-vault-network] by the time I was 20.

I stumbled across Python a few years later, followed by Django, leading
to me working with several of Django's creators and core contributors at
the Lawrence Journal-World. I ended up [authoring Django's `__regex`
QuerySet lookups][django-regex-queryset-lookups][^2] during my time
there, along with various other patches, and maintained the LJW's
internal Django fork (a.k.a. "FrankenDjango").

Later, at The Onion, I authored the (now abandoned)
[django-tagcon][django-tagcon] library, as well as several in-house
modifications for The Onion's internal Django fork; these included a fix
for Django's then-broken timezone support, and a "model shadowing"
facility which worked like the later [custom User model
support][django-auth-custom-user], except it allowed substituting *any*
arbitrary Django model[^3].

While I've learned enough about dozens of different languages over the
past couple of decades to be dangerous — from Haskell to Lisp — I've
always come back to Python. It fits my brain in a way nothing else does
(although I'll admit I wish it were a bit more functional-friendly in
its design). It's the most *readable* language I've ever used (at least
before static type hints showed up[^4]), is amazingly well-documented, has
the best "batteries included" out there, is a near-perfect "glue"
language, and its introspection facilities allow for easily exploring
APIs in an IPython REPL[^5].

I'm quite handy with JavaScript and React as well, along with the
various pieces of a modern JS toolchain like Webpack, Babel, and
PostCSS. And I live and breathe Linux, running it everywhere, including
on my personal ThinkPad. ([Arch][arch-linux], in case you were
wondering.)

I'm available for hire professionally, either via full-time employment
or contract work through my consultancy. Feel free to check out my
[LinkedIn profile][linkedin] for my (extensive!) work history.

## Tools I Use Constantly

- [Arch Linux][arch-linux], operating system
- [i3wm][i3wm], tiling window manager
- [st][suckless-st], terminal
- [tmux][tmux], terminal multiplexer
- [zsh][zsh], shell
  - Although there are days I'm tempted to switch to [Xonsh][xonsh], since
    zsh is ludicrously arcane, and time spent learning its secrets doesn't
    readily transfer to other domains.
- [Neovim][neovim], text editor (heavily customized)
- [Git][git], verson control system
- [fzf][fzf], handy text skimmer
- [Docker][docker], container tool
- [Borg][borg], backup utility
- [Ungoogled-Chromium][ungoogled-chromium], web browser
  - Along with a bunch of extensions, including:
    - Allow Right-Click
    - Browserpass
    - Decentraleyes
    - Stylus
    - [uBlock Origin][ublock-origin] (the most indispensable one, by far)
    - Violentmonkey
- [Python][python], programming language
  - My two most used third-party packages are [IPython][python-ipython]
    and [Pytest][python-pytest].
  - I'm slowly open-sourcing my gobs of utility libraries;
    [Seittik][seittik] is the first stage of this.

(That's not to mention a ridiculous number of bespoke tools I've written
to fit my brain, 99% of them in Python.)

[arch-linux]: https://archlinux.org/
[borg]: https://borgbackup.readthedocs.io/en/stable/index.html
[calver]: https://calver.org/
[django-auth-custom-user]: https://docs.djangoproject.com/en/4.2/topics/auth/customizing/#auth-custom-user
[django-regex-queryset-lookups]: https://docs.djangoproject.com/en/4.2/ref/models/querysets/#regex
[django-tagcon]: https://github.com/rob-b/django-tagcon
[docker]: https://docs.docker.com/
[fzf]: https://github.com/junegunn/fzf
[git]: https://git-scm.com/
[i3wm]: https://i3wm.org/
[ign-vault-network]: https://www.zdnet.com/article/ign-com-will-buy-the-vault-network-5000103354/
[linkedin]: https://www.linkedin.com/in/alchemicalhydra/
[neovim]: https://neovim.io/
[pass-password-manager]: https://www.passwordstore.org/
[postgraphile]: https://github.com/graphile/postgraphile
[postgrest]: https://github.com/PostgREST/postgrest
[project-gemini]: https://gemini.circumlunar.space/
[python]: https://www.python.org/
[python-ipython]: https://ipython.readthedocs.io/en/stable/index.html
[python-pytest]: https://docs.pytest.org/en/latest/index.html
[python-pep-582]: https://peps.python.org/pep-0582/
[seittik]: https://seittik.com/
[suckless-st]: https://st.suckless.org/
[tmux]: https://github.com/tmux/tmux/wiki
[ublock-origin]: https://github.com/gorhill/uBlock
[ungoogled-chromium]: https://github.com/ungoogled-software/ungoogled-chromium
[xonsh]: https://xon.sh/
[zsh]: https://www.zsh.org/

[^1]: Technically, I started with OpenBSD, but over time the lack of
hardware support became a dealbreaker.

[^2]: The commit, if you're curious: https://github.com/django/django/commit/24512a74befc6282a1d299cab452ee9463cc2baa

[^3]: This enabled you to entirely avoid scenarios involving the
`OneToOneField` antipattern for adding fields to an existing model,
since you could rework the expanded model as a single database table.
But the core Django devs and myself tend to disagree on quite a bit, so
upstreaming it never happened.

[^4]: I'm deeply worried about this trend in Python-land. Defenders of
static typing are missing an important tendency when they point out that
typing is "optional"; if history has shown us anything, it's that
features that start out as optional can quickly become compulsory as
they reach a critical mass of popularity.

[^5]: Whenever I try out a new programming language, the first thing I
look for is a REPL with a level of power comparable with what IPython
gives you. Nothing's ever come close.
