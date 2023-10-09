# GeocodeJSON Specification

An attempt to have standard geojson responses from geocoders.

## How to use

Please read the full spec at [master/draft/README.md](https://github.com/jenkin/geocodejson-spec/blob/master/draft/README.md).

You can validate a geocoding service response against this GeocodeJSON spec using the JSON schema provided: [master/draft/geocodejson.schema.json](https://github.com/jenkin/geocodejson-spec/blob/master/draft/geocodejson.schema.json). Refer to [JSON Schema official website](https://json-schema.org/) for further informations.

Please verify the integrity of the JSON schema using the SHA-512 checksum provided: [master/draft/geocodejson.schema.json.checksum](https://github.com/jenkin/geocodejson-spec/blob/master/draft/geocodejson.schema.json.checksum).

## How to contribute

Pre-requisites: [git](https://git-scm.com/), [make](https://www.gnu.org/software/make/), shasum [npx](https://www.npmjs.com/package/npx) (node and npm).

Please follow these steps:

- Let the community knows you want to contibute opening an issue
- Fork this repo, clone it locally and create a new branch
- Install git hooks running `make hooks`
- Extend the [draft document]((https://github.com/jenkin/geocodejson-spec/blob/master/draft/README.md))
- Update the [JSON schema](https://github.com/jenkin/geocodejson-spec/blob/master/draft/geocodejson.schema.json) in `src/` folder
- Run `make build`
- If all is ok, commit your changes and push them
- Open a Pull Request on the main branch of this repo