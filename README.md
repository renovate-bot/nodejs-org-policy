[//]: # "This README.md file is auto-generated, all changes to this file will be lost."
[//]: # "To regenerate it, use `python -m synthtool`."
<img src="https://avatars2.githubusercontent.com/u/2810941?v=3&s=96" alt="Google Cloud Platform logo" title="Google Cloud Platform" align="right" height="96" width="96"/>

# [Organization Policy: Node.js Client](https://github.com/googleapis/nodejs-org-policy)

[![release level](https://img.shields.io/badge/release%20level-general%20availability%20%28GA%29-brightgreen.svg?style=flat)](https://cloud.google.com/terms/launch-stages)
[![npm version](https://img.shields.io/npm/v/@google-cloud/org-policy.svg)](https://www.npmjs.org/package/@google-cloud/org-policy)
[![codecov](https://img.shields.io/codecov/c/github/googleapis/nodejs-org-policy/master.svg?style=flat)](https://codecov.io/gh/googleapis/nodejs-org-policy)




Org policy client for Node.js


A comprehensive list of changes in each version may be found in
[the CHANGELOG](https://github.com/googleapis/nodejs-org-policy/blob/master/CHANGELOG.md).

* [Organization Policy Node.js Client API Reference][client-docs]
* [Organization Policy Documentation][product-docs]
* [github.com/googleapis/nodejs-org-policy](https://github.com/googleapis/nodejs-org-policy)

Read more about the client libraries for Cloud APIs, including the older
Google APIs Client Libraries, in [Client Libraries Explained][explained].

[explained]: https://cloud.google.com/apis/docs/client-libraries-explained

**Table of contents:**


* [Quickstart](#quickstart)
  * [Before you begin](#before-you-begin)
  * [Installing the client library](#installing-the-client-library)
  * [Using the client library](#using-the-client-library)
* [Samples](#samples)
* [Versioning](#versioning)
* [Contributing](#contributing)
* [License](#license)

## Quickstart

### Before you begin

1.  [Select or create a Cloud Platform project][projects].
1.  [Enable billing for your project][billing].
1.  [Enable the Organization Policy API][enable_api].
1.  [Set up authentication with a service account][auth] so you can access the
    API from your local workstation.

### Installing the client library

```bash
npm install @google-cloud/org-policy
```


### Using the client library

```javascript
// Imports the Google Cloud client library

// remove this line after package is released
// eslint-disable-next-line node/no-missing-require
const {OrgPolicyClient} = require('@google-cloud/org-policy');

// TODO(developer): replace with your prefered project ID.
// const projectId = 'my-project'

// Creates a client
// eslint-disable-next-line no-unused-vars
const client = new OrgPolicyClient();

//TODO(library generator): write the actual function you will be testing
async function listConstraints() {
  const constraints = await client.listConstraints({
    parent: `projects/${projectId}`,
  });
  console.info(constraints);
}
listConstraints();

```



## Samples

Samples are in the [`samples/`](https://github.com/googleapis/nodejs-org-policy/tree/master/samples) directory. Each sample's `README.md` has instructions for running its sample.

| Sample                      | Source Code                       | Try it |
| --------------------------- | --------------------------------- | ------ |
| Quickstart | [source code](https://github.com/googleapis/nodejs-org-policy/blob/master/samples/quickstart.js) | [![Open in Cloud Shell][shell_img]](https://console.cloud.google.com/cloudshell/open?git_repo=https://github.com/googleapis/nodejs-org-policy&page=editor&open_in_editor=samples/quickstart.js,samples/README.md) |



The [Organization Policy Node.js Client API Reference][client-docs] documentation
also contains samples.

## Supported Node.js Versions

Our client libraries follow the [Node.js release schedule](https://nodejs.org/en/about/releases/).
Libraries are compatible with all current _active_ and _maintenance_ versions of
Node.js.

Client libraries targeting some end-of-life versions of Node.js are available, and
can be installed via npm [dist-tags](https://docs.npmjs.com/cli/dist-tag).
The dist-tags follow the naming convention `legacy-(version)`.

_Legacy Node.js versions are supported as a best effort:_

* Legacy versions will not be tested in continuous integration.
* Some security patches may not be able to be backported.
* Dependencies will not be kept up-to-date, and features will not be backported.

#### Legacy tags available

* `legacy-8`: install client libraries from this dist-tag for versions
  compatible with Node.js 8.

## Versioning

This library follows [Semantic Versioning](http://semver.org/).






More Information: [Google Cloud Platform Launch Stages][launch_stages]

[launch_stages]: https://cloud.google.com/terms/launch-stages

## Contributing

Contributions welcome! See the [Contributing Guide](https://github.com/googleapis/nodejs-org-policy/blob/master/CONTRIBUTING.md).

Please note that this `README.md`, the `samples/README.md`,
and a variety of configuration files in this repository (including `.nycrc` and `tsconfig.json`)
are generated from a central template. To edit one of these files, make an edit
to its template in this
[directory](https://github.com/googleapis/synthtool/tree/master/synthtool/gcp/templates/node_library).

## License

Apache Version 2.0

See [LICENSE](https://github.com/googleapis/nodejs-org-policy/blob/master/LICENSE)

[client-docs]: https://googleapis.dev/nodejs/org-policy/latest/index.html
[product-docs]: https://cloud.google.com/resource-manager/docs/organization-policy/overview
[shell_img]: https://gstatic.com/cloudssh/images/open-btn.png
[projects]: https://console.cloud.google.com/project
[billing]: https://support.google.com/cloud/answer/6293499#enable-billing
[enable_api]: https://console.cloud.google.com/flows/enableapi?apiid=orgpolicy.googleapis.com
[auth]: https://cloud.google.com/docs/authentication/getting-started
