# Changelog

## [1.33.0](https://github.com/mapfre-tech/arch-ram-reusable-workflows/compare/v1.32.0...v1.33.0) (2026-09-30)


### ⚠ BREAKING CHANGES

* **python:** test-command, dockerfile-path, contract-command and required-middlewares are gone. Projects use the generic layout: sources/ with pyproject.toml, the app package and its tests, and docker/Dockerfile.

### Features

* add container.python.* uv-based reusable workflows ([b3cfafc](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/b3cfafc8eec3add3e9cce77aa6f45d3bf3623b1c))
* added workflows CI for dotnet ([5a15993](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/5a15993bce9ee04604fa0d730774f8ad56526d5f))
* **python:** dockerfile-path as an input in the archetype variants ([6b4d6c7](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/6b4d6c774bbc18c9fe1051526697c5403d5955cb))
* **python:** extension points so the archetype variants can reuse the generic pipeline ([98fd49f](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/98fd49fc0d08c69180a4afb0ee51102416fc610e))
* **python:** variantes de agente y MCP que llaman al genérico de Python sin tocarlo, y workflows de librería ([4c33949](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/4c33949640a40d01ded7d599daca729030c13162))


### Bug Fixes

* **agent:** make the required middlewares configurable, defaulting without ModelCompliance ([caca0a5](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/caca0a5134a55435b85cf0df5c7883b2d26f671e))
* **mcp:** Dockerfile at the repo root, matching the archetype layout ([ad3e17d](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/ad3e17d8e25567d88238839a7dbc588bccb350ff))
* **python:** honour dockerfile-path in the pull-request image build too ([a03e87d](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/a03e87d2dafd3264ff81bac9db110da7bb9f36c0))
* Update accepted values for archetype version file ([65977b1](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/65977b117e3da2942817a38b555e6376425fff44))


### Reverts

* **python:** leave Jose's generic workflows exactly as merged in develop ([1879624](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/1879624777211c92b1aaf8884f849827b7c59dcb))


### Miscellaneous Chores

* release 1.33.0 ([e375213](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/e37521313b0a174c097b0bcc52d8da49f8e27b0e))


### Code Refactoring

* **python:** agent and MCP variants call the generic Python workflows unchanged ([04fd613](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/04fd613b6a097eb365247f5f061db1d6f53ee04e))

## [1.32.0](https://github.com/mapfre-tech/arch-ram-reusable-workflows/compare/v1.31.0...v1.32.0) (2026-09-24)


### Features

* use `ubuntu-latest` as default runner for mirror workflow ([bb810b6](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/bb810b6057affa7397322aa12820d6d6224840e3))

## [1.31.0](https://github.com/mapfre-tech/arch-ram-reusable-workflows/compare/v1.30.0...v1.31.0) (2026-09-21)


### Features

* add karate tests as step ([596d90d](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/596d90dc910c9f46318763d297aff604d478a553))
* karate tests as step ([13024be](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/13024bee73fdfc15ff075ce915d39155f828e028))
* point to v1 version of karate action ([f1ca834](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/f1ca8349f72c89b92e7a6c221a82c823f86603d3))

## [1.30.0](https://github.com/mapfre-tech/arch-ram-reusable-workflows/compare/v1.29.3...v1.30.0) (2026-08-21)


### Features

* **workflows:** soportar carpetas precompiladas entre workflows encadenados ([#303](https://github.com/mapfre-tech/arch-ram-reusable-workflows/issues/303)) ([b6c1164](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/b6c11641f5753fff1479c115904a0cf77650f6a5))

## [1.29.3](https://github.com/mapfre-tech/arch-ram-reusable-workflows/compare/v1.29.2...v1.29.3) (2026-07-29)


### Bug Fixes

* **db.project-manifest.schema:** Added optional property liquibaseVersion ([9d885e1](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/9d885e12dac8bffc403b56033476967d6e9ba02c))

## [1.29.2](https://github.com/mapfre-tech/arch-ram-reusable-workflows/compare/v1.29.1...v1.29.2) (2026-07-24)


### Bug Fixes

* Centralize token management and update release tag validation ([#295](https://github.com/mapfre-tech/arch-ram-reusable-workflows/issues/295)) ([cccf1a0](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/cccf1a030ff67a31d4ed085c526ef11bd525d9eb))

## [1.29.1](https://github.com/mapfre-tech/arch-ram-reusable-workflows/compare/v1.29.0...v1.29.1) (2026-07-14)


### Bug Fixes

* Mainframe - Centralized tokens adoption ([#289](https://github.com/mapfre-tech/arch-ram-reusable-workflows/issues/289)) ([0451701](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/0451701fd2329eac287d37c1f5f94f9cfd523a84))

## [1.29.0](https://github.com/mapfre-tech/arch-ram-reusable-workflows/compare/v1.28.0...v1.29.0) (2026-07-10)


### Features

* remove poetry as package manager by pip in airflow workflows ([#286](https://github.com/mapfre-tech/arch-ram-reusable-workflows/issues/286)) ([d67898c](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/d67898cf8cb1df923548166b1e1d211022c99fd8))


### Bug Fixes

* Improve token-generate error message for centralized vs external token flow ([7ffd62c](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/7ffd62c6c97af126aae77d90b9584cfb88d80fb0))

## [1.28.0](https://github.com/mapfre-tech/arch-ram-reusable-workflows/compare/v1.27.3...v1.28.0) (2026-07-03)


### Features

* Add Mainframe archetype workflows for PR, merge and release processes ([#277](https://github.com/mapfre-tech/arch-ram-reusable-workflows/issues/277)) ([48f3051](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/48f30515220e6b51b6531873874088a55e267bc3))

## [1.27.3](https://github.com/mapfre-tech/arch-ram-reusable-workflows/compare/v1.27.2...v1.27.3) (2026-07-03)


### Bug Fixes

* update GitHub token in API merge commit workflow ([144b478](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/144b478f3453d6b92fd1e016f405e500ed3b8ee4))

## [1.27.2](https://github.com/mapfre-tech/arch-ram-reusable-workflows/compare/v1.27.1...v1.27.2) (2026-06-26)


### Bug Fixes

* Include platform-repo 'arch-bsmar-mk-catalogvalidate' on eda/api ([#270](https://github.com/mapfre-tech/arch-ram-reusable-workflows/issues/270)) ([#273](https://github.com/mapfre-tech/arch-ram-reusable-workflows/issues/273)) ([9770b21](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/9770b21413da08b7d724799f965641af7abf7368))

## [1.27.1](https://github.com/mapfre-tech/arch-ram-reusable-workflows/compare/v1.27.0...v1.27.1) (2026-06-25)


### Bug Fixes

* added component-name text to set image container ([#271](https://github.com/mapfre-tech/arch-ram-reusable-workflows/issues/271)) ([a90dfd1](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/a90dfd19c3f93f8039746373a77cadf8633803e9))

## [1.27.0](https://github.com/mapfre-tech/arch-ram-reusable-workflows/compare/v1.26.0...v1.27.0) (2026-06-24)


### Features

* Prepare library docs for publishing in marketplace ([d82530c](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/d82530c74b11fbfb23b784b80da46e90ec764ce7))


## [1.26.0](https://github.com/mapfre-tech/arch-ram-reusable-workflows/compare/v1.25.0...v1.26.0) (2026-06-23)


### Features

* support optional get-token job and make GH token secrets optional ([#264](https://github.com/mapfre-tech/arch-ram-reusable-workflows/issues/264)) ([b199177](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/b1991776287e0669e8913b95d36ee5b53e24a56a))

## [1.25.0](https://github.com/mapfre-tech/arch-ram-reusable-workflows/compare/v1.24.0...v1.25.0) (2026-06-21)


### Features

* enable git lfs and file size validation for files workflows ([e1af97a](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/e1af97a890bb82e2b3e77183a5b971fe2715617e))

## [1.24.0](https://github.com/mapfre-tech/arch-ram-reusable-workflows/compare/v1.23.0...v1.24.0) (2026-06-10)


### Features

* **PTIZ-334:** add archetype version to manifest schema ([974641a](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/974641adb35b4ba8556411eba8b8909b0fdabbf0))

## [1.23.0](https://github.com/mapfre-tech/arch-ram-reusable-workflows/compare/v1.22.0...v1.23.0) (2026-06-10)


### Features

* add mirror reusable workflow ([f34902e](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/f34902e513617e5dd24ad7fd7bd9335ff9bd75c3))
* mirror.yml as a scalable and configurable reusable workflow ([5b9c8f0](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/5b9c8f01b65c37d7e354c4b2bcfce42018c7446d))
* **PTIZ-334:** add archetype publish reusable workflow ([94d1e93](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/94d1e939bfee78a01ae266e9d252b2ccbe927d15))
* **PTIZ-334:** add archetype publish reusable workflow ([d42b212](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/d42b212d01b5d0a84d2375b0d4ec78db8793c37c))

## [1.22.0](https://github.com/mapfre-tech/arch-ram-reusable-workflows/compare/v1.21.2...v1.22.0) (2026-05-11)


### Features

* add reusable workflows and schemas for npm library archetype ([2667eb8](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/2667eb8e51d30f6e5d1462a593f71d60de8349ad))
* add reusable workflows for npm library archetype ([a28b926](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/a28b926032438186fc2be67f07828bdb05b9c5c8))
* Mejora en la validación de esquemas para workflows reutilizables ([0f51eda](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/0f51edaeb96c1004955ead3184b2bbcc4b87c272))
* update README install snippet on release ([74693cf](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/74693cfdf534362637ea6e40099bfcf9f696b002))


### Bug Fixes

* generate package-lock.json if missing before npm ci ([a3eeb9a](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/a3eeb9a526e90b1aeaaf081278f7aaa07c79ba02))
* point to bugfix branch ([#229](https://github.com/mapfre-tech/arch-ram-reusable-workflows/issues/229)) ([33eb534](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/33eb53400315ab4efdb7e800bb60eca2fd30c9cd))
* remove hardcoded npm cache config from setup-node ([04531df](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/04531df6a55cbeab86db099536450a6ec6ad1a6f))

## [1.21.2](https://github.com/mapfre-tech/arch-ram-reusable-workflows/compare/v1.21.1...v1.21.2) (2026-03-25)


### Bug Fixes

* Añadir contenedor sonar-scanner-cli al workflow de MongoDB ([#213](https://github.com/mapfre-tech/arch-ram-reusable-workflows/issues/213)) ([09aa99f](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/09aa99f94971c85078cc8e4f909ff942c6e64439))
* api.project-manifest schema — publish_api_json optional y añadir propiedad definition ([c406484](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/c40648400dd214d0aba7e2966a6149baf002f8bb))

## [1.15.4](https://github.com/mapfre-tech/arch-ram-reusable-workflows/compare/v1.15.3...v1.15.4) (2026-xx-xx)

### Bug Fixes

   * fix schema api.project-manifest: publish_api_json deja de ser required y se añade propiedad definition ([#222](https://github.com/mapfre-tech/arch-ram-reusable-workflows/pull/222))


## [1.21.1](https://github.com/mapfre-tech/arch-ram-reusable-workflows/compare/v1.21.0...v1.21.1) (2026-03-21)


### Bug Fixes

* revert action-java-maven to v1 in container.gaia.merge-commit.yml ([710433f](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/710433f59864e0b604b306c013bfee7494f0b26a))
* revert action-java-maven to v1 in container.gaia.pull-request.yml ([10e4078](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/10e40789d3da7f73569a476cba27fe17a52d8f7f))
* revert action-java-maven to v1 in container.java.merge-commit.yml ([2fdfd33](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/2fdfd332c616d37b5524097a3a5649a442c00971))
* revert action-java-maven to v1 in container.java.pull-request.yml ([37c6579](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/37c6579306afc5cd9b4d51fdf96284e619c79df1))
* revert action-java-maven to v1 in gaia.merge-commit.yml ([ae63612](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/ae636122ea2e150c72d550b003f955f68285f766))
* revert action-java-maven to v1 in gaia.pull-request.yml ([c218732](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/c2187321e96ad9d259b951605f17f6fe3d2440a4))
* revert action-java-maven to v1 in lib.java.merge-commit.yml ([26661e2](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/26661e259f5b03bf393bb81062ba46f10447693e))
* revert action-java-maven to v1 in lib.java.pull-request.yml ([0a733ab](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/0a733abf0f756d0a004d3c39598def6b29cf7066))
* Revert mapfre-tech/action-java-maven from v2 to v1 ([57b282e](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/57b282e65eeb590edc45848c97637cae9dc9fb47))

## [1.21.0](https://github.com/mapfre-tech/arch-ram-reusable-workflows/compare/v1.20.0...v1.21.0) (2026-03-21)


### Features

* **workflows:** añadir lib.arch.java.pull-request.yml ([#202](https://github.com/mapfre-tech/arch-ram-reusable-workflows/issues/202)) ([19b70e2](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/19b70e26e715bd532f1022ead5cb6a4970979fc5))

## [1.20.0](https://github.com/mapfre-tech/arch-ram-reusable-workflows/compare/v1.19.3...v1.20.0) (2026-03-21)


### Features

* **workflows:** exponer security.yml como workflow_call reusable para equipos ([#201](https://github.com/mapfre-tech/arch-ram-reusable-workflows/issues/201)) ([b6c0e87](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/b6c0e87e966752dc7fc2cb809a4a6e4fad596f08)), closes [#195](https://github.com/mapfre-tech/arch-ram-reusable-workflows/issues/195)


### Bug Fixes

* **workflows:** corregir input next-snapshot-create-pull-request sin efecto en lib.java ([#200](https://github.com/mapfre-tech/arch-ram-reusable-workflows/issues/200)) ([90647e6](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/90647e628301ad8c63ef89e34cfe4612b8ac2167)), closes [#193](https://github.com/mapfre-tech/arch-ram-reusable-workflows/issues/193)

## [1.19.3](https://github.com/mapfre-tech/arch-ram-reusable-workflows/compare/v1.19.2...v1.19.3) (2026-03-10)


### Bug Fixes

* Enhance SNAPSHOT promotion workflow and fix related issues ([8d0af14](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/8d0af1475f5cf6768c6834ad9d605d16635bd16b))


## [1.19.2](https://github.com/mapfre-tech/arch-ram-reusable-workflows/compare/v1.19.1...v1.19.2) (2026-01-20)


### Bug Fixes

* **merge-commit:** Añadido parámetro booleano `is-fix` en workflows de merge-commit para indicar si la promoción es para una versión fix ([cfca1b5](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/cfca1b5e487c9457c413fa0bc12774c7a783888e))

## [1.19.1](https://github.com/mapfre-tech/arch-ram-reusable-workflows/compare/v1.19.0...v1.19.1) (2026-01-19)


### Bug Fixes

* Fix step to add coverage badge in readme ([#183](https://github.com/mapfre-tech/arch-ram-reusable-workflows/issues/183)) ([4ba3994](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/4ba3994926fa921f3c2b3fc2fd85ff67995ec70d))

## [1.19.0](https://github.com/mapfre-tech/arch-ram-reusable-workflows/compare/v1.18.0...v1.19.0) (2026-01-15)


### Features

* **workflows:** se añaden workflows para librerías Javas y Python basadas en Conventional Commits ([afedbc3](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/afedbc3576237ad44537c3fe67298921d3658a6d))

## [1.18.0](https://github.com/mapfre-tech/arch-ram-reusable-workflows/compare/v1.17.1...v1.18.0) (2025-12-12)


### Features

* added v2 archetype ([8a809ce](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/8a809ce9a146d5dff3d2f97c50f07bcd5dc1983b))
* added workflows arqos ([b7f7090](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/b7f70902d13ba8b2a71f4853368e198593ced605))

## [1.17.1](https://github.com/mapfre-tech/arch-ram-reusable-workflows/compare/v1.17.0...v1.17.1) (2025-12-11)


### Bug Fixes

* wrong reference to build and push action on acr ([0b51d59](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/0b51d59557f54535887ba6b4c0e076d6a32b8170))

## [1.17.0](https://github.com/mapfre-tech/arch-ram-reusable-workflows/compare/v1.16.0...v1.17.0) (2025-11-27)


### Features

* se añade workflow reusable para arquetipo POI ([e7f97d3](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/e7f97d3767de25f8690f71f249952c15617f610b))

## [1.16.0](https://github.com/mapfre-tech/arch-ram-reusable-workflows/compare/v1.15.4...v1.16.0) (2025-11-12)


### Features

* cambios en el workflow de api para agilizar el proceso de publicación ([d87b170](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/d87b170c95888a30056dcde6ee30ec81dbfee230))
* update PR workflow for dinamic sonar host and version ([#41](https://github.com/mapfre-tech/arch-ram-reusable-workflows/issues/41)) ([38040dd](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/38040dd930319e7e40fb953b114fdae355fea207))

## [1.15.4](https://github.com/mapfre-tech/arch-ram-reusable-workflows/compare/v1.15.3...v1.15.4) (2025-10-22)


### Bug Fixes

* build-args en action-azure v2 ([c83c3ee](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/c83c3ee76915ff732421674f62511a91ff83c483))

## [1.15.3](https://github.com/mapfre-tech/arch-ram-reusable-workflows/compare/v1.15.2...v1.15.3) (2025-10-15)


### Bug Fixes

* included optional clean parameter for publish artifact ([4ea7d8a](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/4ea7d8a3254aeab677f7efdc5ae3c65feb6ea69a))

## [1.15.2](https://github.com/mapfre-tech/arch-ram-reusable-workflows/compare/v1.15.1...v1.15.2) (2025-09-26)


### Bug Fixes

* included credentials azure artifacts necessary for read pom artifacts ([#113](https://github.com/mapfre-tech/arch-ram-reusable-workflows/issues/113)) ([9c608b6](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/9c608b6bdbe4d5448509e7f0a9a12d2b9bea45cd))

## [1.15.1](https://github.com/mapfre-tech/arch-ram-reusable-workflows/compare/v1.15.0...v1.15.1) (2025-09-18)


### Bug Fixes

* fixed bug schemas libjava ([#109](https://github.com/mapfre-tech/arch-ram-reusable-workflows/issues/109)) ([ca70046](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/ca70046f97cca343e736e4af8acde3a9a1b6d2dc))


## [1.15.0](https://github.com/mapfre-tech/arch-ram-reusable-workflows/compare/v1.14.1...v1.15.0) (2025-09-12)


### Features

* Batch Airflow workflows ([#102](https://github.com/mapfre-tech/arch-ram-reusable-workflows/issues/102)) ([be7d0cb](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/be7d0cbadefab56c1f603187ce9066f06cb9a4e5))

## [1.14.1](https://github.com/mapfre-tech/arch-ram-reusable-workflows/compare/v1.14.0...v1.14.1) (2025-09-10)


### Bug Fixes

* Build: mvn install ([528e9ac](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/528e9ac21d5769e8deaea8002ffae26505a1aa93))

## [1.14.0](https://github.com/mapfre-tech/arch-ram-reusable-workflows/compare/v1.13.4...v1.14.0) (2025-09-04)


### Features

* included workflows CI for GAIA applications in container ([2ce0d5a](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/2ce0d5aedc4511efb3217706765882efd77e09cf))

## [1.13.4](https://github.com/mapfre-tech/arch-ram-reusable-workflows/compare/v1.13.3...v1.13.4) (2025-08-29)


### Bug Fixes

* add option to skip tests in workflows GAIA ([#93](https://github.com/mapfre-tech/arch-ram-reusable-workflows/issues/93)) ([19afdde](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/19afdde993ecadd055c575051c69e2245eb95aeb))

## [1.13.3](https://github.com/mapfre-tech/arch-ram-reusable-workflows/compare/v1.13.2...v1.13.3) (2025-08-26)


### Bug Fixes

* changed step build in GAIA workflows from package to install ([6611d1c](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/6611d1cff63e840c24ce295a06ffba17d1b31fb5))

## [1.13.2](https://github.com/mapfre-tech/arch-ram-reusable-workflows/compare/v1.13.1...v1.13.2) (2025-08-18)


### Bug Fixes

* Prepare-release before generate AsyncAPI -&gt; to remove -snapshot … ([8c15338](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/8c153382e274e82dcceae80c162301bd0e1fa622))
* Prepare-release before generate AsyncAPI -&gt; to remove -snapshot suffix ([8062189](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/80621898f46959fae126e20d15b42469c228813f))
* Prepare-release before generate AsyncAPI -&gt; to remove -snapshot suffix in generated template ([1c846fa](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/1c846fa284017d048e2e851dcba5f949c4e74f52))

## [1.13.1](https://github.com/mapfre-tech/arch-ram-reusable-workflows/compare/v1.13.0...v1.13.1) (2025-07-22)


### Bug Fixes

* Publish Event API only on RELEASE ([cafef9b](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/cafef9be02fcdf8f0913e8378748c517aa783fbd))
* Publish Event API only on RELEASE ([fc805e5](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/fc805e5f8a06b1dd5cddf9233476362f10689ebf))
* Publish Event API only on RELEASE ([1d3a108](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/1d3a1085b69d1c5bc7efa8da7b4a75d9f04d7368))

## [1.13.0](https://github.com/mapfre-tech/arch-ram-reusable-workflows/compare/v1.12.0...v1.13.0) (2025-07-17)


### Features

* Validación de reglas spectral EDA ([72126a0](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/72126a091d2d0efba9691e7fcc7457f3fba4a076))
* Validación de reglas spectral EDA ([de3961d](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/de3961d2901bfdac833533ad9b22583199cd50a2))

## [1.12.0](https://github.com/mapfre-tech/arch-ram-reusable-workflows/compare/v1.11.1...v1.12.0) (2025-07-16)


### Features

* publicación marketplace API-EDA ([0b9b56a](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/0b9b56ae89799c879d708be79194d44883e67142))
* publicación marketplace API-EDA ([dc0d183](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/dc0d1839e9876cfe68c1ba311a39462d32c87e35))

## [1.11.1](https://github.com/mapfre-tech/arch-ram-reusable-workflows/compare/v1.11.0...v1.11.1) (2025-07-15)


### Bug Fixes

* **lib-java:** problem with control jobs ([8c5d338](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/8c5d3380b4cb864c5b4011d40ea066e4ef29e61c))

## [1.11.0](https://github.com/mapfre-tech/arch-ram-reusable-workflows/compare/v1.10.0...v1.11.0) (2025-07-01)


### Features

* added reusable workflows for java lib ([65c7518](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/65c75182e95066326b05a6d04bd265b7cd6e207c))

## [1.10.0](https://github.com/mapfre-tech/arch-ram-reusable-workflows/compare/v1.9.0...v1.10.0) (2025-06-27)


### Features

* improve output-style logs and do not set app mobile secrets as required ([#64](https://github.com/mapfre-tech/arch-ram-reusable-workflows/issues/64)) ([d6d0784](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/d6d07847354a411b6415041e7fc2fc62a021e053))
* Lib sources authentication and secrets for docker push in merge ([d136e82](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/d136e8261773ecac3befeb1a05136927f8dd474e))
* Reusable workflows for django libs ([#65](https://github.com/mapfre-tech/arch-ram-reusable-workflows/issues/65)) ([eb426ac](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/eb426ac1cefd4c1d15d6df3afb7c6402d98709a4))

## [1.9.0](https://github.com/mapfre-tech/arch-ram-reusable-workflows/compare/v1.8.0...v1.9.0) (2025-06-25)


### Features

* added workflows reusable for no-sql archetype ([ac40a97](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/ac40a97794409456ea3e61acf7e249cebedea71b))


### Bug Fixes

* included step commit in relational workflow merge-commit ([ac40a97](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/ac40a97794409456ea3e61acf7e249cebedea71b))

## [1.8.0](https://github.com/mapfre-tech/arch-ram-reusable-workflows/compare/v1.7.0...v1.8.0) (2025-06-16)


### Features

* add files workflow ([#55](https://github.com/mapfre-tech/arch-ram-reusable-workflows/issues/55)) ([b071607](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/b07160794bc84fb37cf4c6207f5647d4df49d792))

## [1.7.0](https://github.com/mapfre-tech/arch-ram-reusable-workflows/compare/v1.6.1...v1.7.0) (2025-06-06)


### Features

* added workflows for GAIA archetype ([8bc1986](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/8bc198638c778c32642f1dd8e35a6a7e9556123d))


### Bug Fixes

* added input runs-on-sonar for all pull request wworkflows ([#50](https://github.com/mapfre-tech/arch-ram-reusable-workflows/issues/50)) ([7f40f68](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/7f40f68e79f7cac2d05427e04c023f6b09841323))

## [1.6.1](https://github.com/mapfre-tech/arch-ram-reusable-workflows/compare/v1.6.0...v1.6.1) (2025-06-06)


### Bug Fixes

* [BUG-65] Flujo api.merge-commit en tag v1 ([#47](https://github.com/mapfre-tech/arch-ram-reusable-workflows/issues/47)) ([7fa2a75](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/7fa2a7558fccf313b83f660b977f87e9270467fc))

## [1.6.0](https://github.com/mapfre-tech/arch-ram-reusable-workflows/compare/v1.5.0...v1.6.0) (2025-06-02)


### Features

* add missing FIREBASE_TOKEN ([904ff6c](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/904ff6c4d07716e1c2769ad3e6ed82094760eac8))
* add nx-target-app-name in the schema and configure needs init ([f8051d8](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/f8051d83d479ae9d0d123880b053ba9aa1878bd0))
* align reusable workflow with latest archetype ([e926034](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/e9260345c512f6966dd2c8d54f15118348844521))
* checkout in merge commit with ram github token ([a407654](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/a40765478d8fff9bea1eda680c5d7ec91cd4d863))
* conditionally execute mobile app jobs based on capacitor config ts ([9248572](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/9248572573927323eb20460ccd73794cd9e0151c))
* improve needs condition execution ([ac14951](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/ac14951f9f0bc6a91a21af126bcdac8dd4cb7878))
* improve workflow to only run decode of the existing env variable ([9b11c0b](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/9b11c0b181dfe777806be25540e290c64c07e597))
* include basic workflow validator ([79c3000](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/79c30003f2bb527ae215cf215f95b417fcf37ca9))
* MAR-569 Actualización del reusable enfoque plataforma ingeniería arquetipo sdm aplicaciones móviles ([116aabb](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/116aabb6f7813589e1b922a3d8d4bdc9c9efe714))
* Only install azure-cli on macos machine if not installed ([5efe555](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/5efe555aa9f2fd59616dfcf400d036f275167aed))
* organize env variables for ios and android steps ([987fee7](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/987fee76e03b79fc51b78ab0c0d324b0e7a78d12))
* point to MAR569 deploy schema ([8235f90](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/8235f90be0f50b39495944ff1b272605fab591da))
* receive docker registry credentials ([ab81833](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/ab81833af1f2ba4d1d8ae8b3577ea8927b4f4801))
* Update bundle config to resolve github authentication to fastlane ([a61797b](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/a61797bfc1df655f05fffbc72f21bcf5fb909ab7))
* update pointer to google services account json env var ([4d7725f](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/4d7725f2685e132af9ba2bf4d40399b21104851c))
* update pull request workflow ([9547744](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/9547744b379100056c31ffbc849fb878bf26a30e))
* update release web step with docker credentials ([da6ff93](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/da6ff93c46f5d3c7cd6cbae8af624d83fce6b34a))
* update validate schema pointer ([e6f168f](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/e6f168f5a86cb8683f19a6115d1f0ea208339c32))
* update workflow executions to latest changes ([76feb81](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/76feb81a22487d3e18c4bf45370b696ef87feefb))
* update working workflow to use latest archetype ([154e3cf](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/154e3cfe315df944617ef2ef06ba78925c1d5470))

## [1.5.0](https://github.com/mapfre-tech/arch-ram-reusable-workflows/compare/v1.4.0...v1.5.0) (2025-05-06)


### Features

* Added context-filter param ([46b0cce](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/46b0cce2ad585ed7d9f29130ef20b14ab20ae7ad))
* db.relational Workflows ([afc74db](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/afc74db2933c0480b8dd1b0b6a4f841dc30f2de0))
* tagDatabase changesets are not allowed ([581c7fd](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/581c7fd731aa0183b771a8db027ad44983cc3321))


### Bug Fixes

* copìlot PR issues ([bf8fa97](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/bf8fa976ca64dc7dd0935f2d5c7baad3d5c469be))
* db.relation pull request create-config ([7cd3a3e](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/7cd3a3e3521165db32194363dd066a8e8e3ba991))
* error in jq next-release-version ([b2902bb](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/b2902bb37debc3f1575c2eaff7fe42bfa9b9be13))
* invalid changesets message ([2790756](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/2790756145d41e176a016b835b72219e34cafd65))

## [1.4.0](https://github.com/mapfre-tech/arch-ram-reusable-workflows/compare/v1.3.0...v1.4.0) (2025-04-25)


### Features

* Added python CI workflows ([10124d9](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/10124d998f634bd381fcb662f16af5bead6c925c))

### Bug Fixes

* changed env.RAM_GITHUB_GIT_TOKEN for secrets.RAM_GITHUB_GIT_TOKEN ([2eb0983](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/2eb09834bb2af5cbd021c9e21eae77dd3419e810))
* force to use token with owner permissions ([2eb0983](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/2eb09834bb2af5cbd021c9e21eae77dd3419e810))

## [1.3.0](https://github.com/mapfre-tech/arch-ram-reusable-workflows/compare/v1.2.0...v1.3.0) (2025-04-11)


### Features

* Añadido workflows reusables para EDA y mejora en los workflows de API añadiendo el nuevo fichero project-manifest.json ([0dd8757](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/0dd8757b266e2493c30a70493edaee72171388be))

## [1.2.0](https://github.com/mapfre-tech/arch-ram-reusable-workflows/compare/v1.1.2...v1.2.0) (2025-04-11)


### Features

* Get reusable workflow ref dynamically ([fc900c2](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/fc900c28c5af0d215d0efbe61fbaea4a05fdf9af))

## [1.1.2](https://github.com/mapfre-tech/arch-ram-reusable-workflows/compare/v1.1.1...v1.1.2) (2025-04-05)


### Bug Fixes

* Update validate-workflow.yml ([f2a6749](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/f2a674904c377c85da78ff32a2a77078c7a39dbe))

## [1.1.1](https://github.com/mapfre-tech/arch-ram-reusable-workflows/compare/v1.1.0...v1.1.1) (2025-04-05)


### Bug Fixes

* default schema validation to v1 ([4a07d43](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/4a07d4375bcade00ccc081390db3e2f1a9e6af95))
* default schema validation to v1 ([ff72e1a](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/ff72e1a52b01965871b1e63f2e6f8443b779b660))

## [1.1.0](https://github.com/mapfre-tech/arch-ram-reusable-workflows/compare/v1.0.0...v1.1.0) (2025-04-04)


### Features

* parametrizado runs-on a usar en job de sonar ([7d750f5](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/7d750f5e9a116265922ab473c4c0e4c127e98717))

## 1.0.0 (2025-03-31)


### Features

* added merge commit workflow ([fa75e66](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/fa75e6620018e32316e6b8151e3f704f46c3483b))
* container java workflows ([832cf56](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/832cf56a6c66addfc672be7717114f05a142d509))
* workflows reusable for api ([611561b](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/611561b237bc8a8de0779f700e031aa2202fb5ea))


### Bug Fixes

* added parameters optional to java action and snapshot next promotion ([ecc9b93](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/ecc9b93f86196ab7877d6a32a5730386ddbec9a9))
* container.java.pull-request.schema.yml ([56ee929](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/56ee929599342c8e61411195200e9721baef1fc3))
* extract url host sonar ([4b31c0a](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/4b31c0a315127b3ad451edc7bf8abf7e3b51b962))
* extract url host sonar ([a28e6bd](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/a28e6bd75b3e0f6add8114c14063adf1745d4b32))
* GH_GIT_TOKEN secret ([d02b2e6](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/d02b2e62648c904f1b45dedeb6675c11a93338a5))
* lowercase inputs ([058a9c6](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/058a9c6307032d3c42e09317c4f52cf29be30f53))
* removed if condition in validate-workflow ([1daeb09](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/1daeb09514fa1135018d7fecb0df35ed31c28e83))
* scanMetadataReportFile ([f525bdb](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/f525bdb544b5a0693a5fedd5f427da72219455dc))
* typo error ([857c076](https://github.com/mapfre-tech/arch-ram-reusable-workflows/commit/857c076e2e0fd42c3308af94feea0b03aba75c8d))
