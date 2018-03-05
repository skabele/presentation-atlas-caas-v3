# atlas-caas-v3 & caas-spinner-ts

ARTICULATE & SPEAK SLOWLY

## Intro

1. summary of presentation (show few main points on screen)
2. why `atlas-caas-v3` - our DRY attempt
    1. develop CaaS faster
    2. more maintainable & extensible
    3. keep uniformity across implementations 
    4. keep ourselves motivated
3. show `atlas-caas-v3/src/caas-service.ts`

## Spinned FooBar project

1. show new `foobar` project created using `caas-spinner-ts`
    * thank for spinner idea
    * note: spinning tested in Docker
2. **infrastructure**
    * comment on `foobar/src/index.ts` - starting application by `service.createServer()`
    * logging
    * error handling (with validations errors)
    * NewRelic
    * default edpoints (livecheck, version)
3. **main features** - show in code how it delegates heavy lifting to `atlas-caas-v2`
    * generic label
    * manifestation using stream processing of `shipments.json`
    * summary and detail manifest documents
    * validation of request
    * profile
4. **extra helpers** - comment on `atlas-caas-v3/src/index.ts`:
    * ... ?
    * `labels.removeDefaultsFromXamlTemplate`
5. **extensibility / maintainability**    
    * possibility to fix / enhance manifesting
    * add security enhancements like like [helmet](https://www.npmjs.com/package/helmet) 
    * add new common endpoint
    * add profile validation
    * ... of course, there is maintenance cost

## Real implementations

1. present Nacex
2. mention GLS

## Other & closing

1. TS and JS
    * atlas-caas-v3 is usable in both TS and JS. Type annotations can be helpfull even in JS
    * caas-spinner-ts spins TS project, but you can grab JS skeleton in `./js/` after compilation
    * comment how we use TS (prefer interfaces over classes)
2. **OPTIONAL** show GLS migration to atlas-caas-v3 (size of code, dependencies)
3. **OPTIONAL** Demo usefulness of types in IDE   
    * show editing code in TS with type safety
    * show type hints in JS
4. Maintaining atlas-caas-v3:
    * semver, README, CHANGELOG    
    * ready to use
    * we are happy to support anybody who would like to try it (in TS or in JS)
5. Request for feedback

