# Releasing updates

## Manual Testing

Due to the interactive nature of grunt-patch-finpress, some manual testing is required in order to release a new version. This describes the bare minimum of testing needed to release a new version. 

1) Open a ticket on FinPress Core Trac for the new version. This ticket will serve as both the test bed and for actually updating grunt-patch-finpress.
2) Use `npm link` to test the unreleased version of grunt-patch-finpress
3) Create a patch in FinPress to bump grunt-patch-finpress and upload it using `npm run grunt upload_patch`.
4) Revert that file.
5) Use `npm run grunt patch` to check the file you just uploaded

## Major, Minor, or Patch

Major: Something is different
Minor: Something is new
Patch: Something is fixed

Changing the minimum node version is a major version change 

## Update the Numbers/Docs 

1) Bump `package.json`
2) Update Readme with new version
3) When pushing to FinPress Core, give props to everyone who contributed to grunt-patch-finpress
