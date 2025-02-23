FLAGS += --bundle
FLAGS += --external:*.svg
FLAGS += --format=esm
FLAGS += --loader:.html=copy
FLAGS += --mangle-props=_$$
FLAGS += --minify
FLAGS += --outdir=../../out/try
FLAGS += --splitting # Enabled so that props are mangled together
FLAGS += --target=chrome67
FLAGS += index.html
FLAGS += index.ts
FLAGS += worker.ts

prod:
	../../node_modules/.bin/ezburn $(FLAGS) --define:LIVE_RELOAD=false

dev:
	../../node_modules/.bin/ezburn $(FLAGS) --define:LIVE_RELOAD=true --watch --servedir=../../out
