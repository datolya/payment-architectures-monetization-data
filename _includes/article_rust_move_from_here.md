
DATA SYSTEMS DESIGN
Let's set up a test repository.

Let's use `uv` since it's much faster than poetry! 
We want to use the rust revolution to our advantage.

Steps:

install rust with rustup

```
-> cargo (Rust package manager) needs to be present on our machine
--> create requirements.in
---> uv pip compile requirements.in -o requirements.txt
```

/ Here uv automatically generates our .txt with comments on dependencies
```
uv pip install -r requirements.txt
```

/ Make sure the .venv is correctly set for pycharm (repository root and correct Python version)

Note that uv treates req.txt AS THE LOCKFILE ITSELF. So we commit it with the repo and that's it.

Use another clever Rust tool for linting!!!
```
ruff format .
ruff check --fix
```

