# ABK_repo
AnyBase Kernel external module repo.

`abk-modules.json` is the central build-module catalog for the ABK app.

Rules:

- Regular module entries use `"kind": "module"`.
- Module-set entries use `"kind": "module_set"`.
- The catalog only declares the module-set entrypoint.
- Child feat/fix definitions are read from the target repository `module.conf`.
- The app expands module-set children into workflow inputs, but the workflow
  still receives a flat string list.
