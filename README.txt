See https://github.com/google-ai-edge/model-explorer for the original repo.

I wanted to run this tool on windows directly without having to use WSL.  At time of writing,
this isn't supported by the original repo.

Since it's only the adapters that they depend on which creates this restriction, and I didn't need
any of the adapters I took the wheel's source code and made this repo from it.  I also took out
some of the code that relied on torch graph exporting with the remaining portions handled by
monkey patching in the downstream library/application.

If you have a similar use case, I wouldn't recommend using this repo - I probably broke some stuff.
