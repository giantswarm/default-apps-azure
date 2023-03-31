<!--
Not all PRs will require all tests to be carried out. Delete where appropriate.
-->

<!--
MODIFY THIS AFTER your new app repo is in https://github.com/giantswarm/github
@team-halo-engineers will be automatically requested for review once
this PR has been submitted. (But not for drafts)
-->

This PR:

- adds/changes/removes etc

### Testing

Description on how default-apps-azure can be tested.

- [ ] fresh install works
  - [ ] AWS
  - [ ] Azure
  - [ ] KVM
- [ ] upgrade from previous version works
  - [ ] AWS
  - [ ] Azure
  - [ ] KVM

#### Other testing

Description of features to additionally test for default-apps-azure installations.

- [ ] check reconciliation of existing resources after upgrading
- [ ] X still works after upgrade
- [ ] Y is installed correctly

<!--
Changelog must always be updated.
-->

### Checklist

- [ ] Update changelog in CHANGELOG.md.
- [ ] Make sure `values.yaml` and `values.schema.json` are valid.

### Trigger e2e tests

<!--
If for some reason you want to skip the e2e tests, remove the following lines.
-->

/run cluster-test-suites
