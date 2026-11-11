# PLANOMIX — live demo

The hosted build of the merchandising simulator. Everything here runs in the browser:
the 3D floor, the fitted purchase-probability surface, the scenario editor and the
1,000-plan search.

This repository holds only the static site, which is exactly what the page already
serves to anyone who opens it. The training pipeline, the vision server and the model
code are not part of it.

**Reading a store from photographs is not available here.** That path calls a model
through a local CLI, so it needs the project's own server rather than a static host.
Everything else works as it stands.

    web/data/*.json   exported by the training run: the response surface,
                      the demo floor, and the held-out validation results
    scene.js          the isometric floor, drawn procedurally
    archetypes.js     floor archetypes, and what each store type has to fight over
    app.js            the five screens, scoring, and the scenario search
