# Install cedarpy

(DRAFT)

TODO
- Give examples for each to test things out
- Provide screenshots
- Link to related videos

## Cedar Python

The official Cedar implementation is in Rust,
  and many Cedar docs are explained using Rust examples.
Rust is fantastic,
  but it also has its own steep learning curve and
  can be overkill for some projects.
Lucky for us,
  [cedarpy](https://github.com/k9securityio/cedar-py)
  provides Python bindings to
  the official Cedar implementation!

However, if you're in OS X and just follow
the cedarpy installation instructions:

```
  $ pip install cedarpy
```

you'll probably get an error like:

```
% pip3 install cedarpy                                                       
error: externally-managed-environment
                                                                             
× This environment is externally managed                        
╰─> To install Python packages system-wide, try brew install
    xyz, where xyz is the package you are trying to
    install.
```

The trick is to first set up a virtual environment
so we can install a local version of cedarpy independent
of the system Python installation:

```
$ python3 -m venv .venv
$ source .venv/bin/activate
$ pip3 install cedarpy
```

## Cedar CLI

```
$ cargo install cedar-policy-cli
```

## Cedar VSCode Extension

[Install the Cedar Policy Extension in VSCode](https://marketplace.visualstudio.com/items?itemName=cedar-policy.vscode-cedar)

