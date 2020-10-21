# devops-netology2.4

## 1.	git show aefea

commit aefead2207ef7e2aa5dc81a34aedf0cad4c32545
Author: Alisdair McDiarmid <alisdair@users.noreply.github.com>
Date:   Thu Jun 18 10:29:58 2020 -0400

    Update CHANGELOG.md

## 2.	git show 85024d3

v0.12.23

## 3.	git show b8d720

commit 56cd7859e05c36c06b56d013b55a252d0bb7e158
Merge: 58dcac4b7 ffbcf5581

## 4.	git log v0.12.23..v0.12.24 --oneline

33ff1c03b (tag: v0.12.24) v0.12.24
b14b74c49 [Website] vmc provider links
3f235065b Update CHANGELOG.md
6ae64e247 registry: Fix panic when server is unreachable
5c619ca1b website: Remove links to the getting started guide's old location
06275647e Update CHANGELOG.md
d5f9411f5 command: Fix bug when using terraform login on Windows
4b6d06cc5 Update CHANGELOG.md
dd01a3507 Update CHANGELOG.md
225466bc3 Cleanup after v0.12.23 release

## 5.	 git grep --show-function providerSource

Homework2.4.md=Date:   Thu Mar 5 21:12:06 2020 +0000
Homework2.4.md:5.       git log -SproviderSource
Homework2.4.md=index 2f6ac1a91..751844e17 100644
Homework2.4.md:+       providerSource := allVersions.ID
command/import_test.go=func TestImport_remoteState(t *testing.T) {
command/import_test.go: providerSource, close := newMockProviderSource(t, map[string][]string{
command/import_test.go:         ProviderSource:   providerSource,
command/import_test.go=func TestImport_initializationErrorShouldUnlock(t *testing.T) {
command/import_test.go: providerSource, close := newMockProviderSource(t, map[string][]string{
command/import_test.go:         ProviderSource:   providerSource,
command/import_test.go=func TestImportModuleVarFile(t *testing.T) {
command/import_test.go: providerSource, close := newMockProviderSource(t, map[string][]string{
command/import_test.go:         ProviderSource:   providerSource,
command/import_test.go=func TestImportModuleInputVariableEvaluation(t *testing.T) {
command/import_test.go: providerSource, close := newMockProviderSource(t, map[string][]string{
command/import_test.go:         ProviderSource:   providerSource,
command/init_test.go=func TestInit_getProvider(t *testing.T) {
command/init_test.go:   providerSource, close := newMockProviderSource(t, map[string][]string{
command/init_test.go:           ProviderSource:   providerSource,
command/init_test.go=func TestInit_getProviderSource(t *testing.T) {
command/init_test.go:   providerSource, close := newMockProviderSource(t, map[string][]string{
command/init_test.go:           ProviderSource:   providerSource,
command/init_test.go=func TestInit_getProviderInLegacyPluginCacheDir(t *testing.T) {
command/init_test.go:   providerSource := getproviders.MultiSource{}
command/init_test.go:           ProviderSource: providerSource,
command/init_test.go=func TestInit_getProviderLegacyFromState(t *testing.T) {
command/init_test.go:   providerSource, close := newMockProviderSource(t, map[string][]string{
command/init_test.go:           ProviderSource:   providerSource,
command/init_test.go=func TestInit_getProviderInvalidPackage(t *testing.T) {
command/init_test.go:   providerSource := getproviders.NewMockSource([]getproviders.PackageMeta{meta}, nil)
command/init_test.go:           ProviderSource:   providerSource,
command/init_test.go=func TestInit_getProviderDetectedLegacy(t *testing.T) {
command/init_test.go:   providerSource, psClose := newMockProviderSource(t, map[string][]string{
command/init_test.go:           {Source: providerSource},
command/init_test.go:func TestInit_providerSource(t *testing.T) {
command/init_test.go:   providerSource, close := newMockProviderSource(t, map[string][]string{
command/init_test.go:           ProviderSource:   providerSource,
command/init_test.go=func TestInit_cancel(t *testing.T) {
command/init_test.go:   providerSource, closeSrc := newMockProviderSource(t, map[string][]string{
command/init_test.go:           ProviderSource:   providerSource,
command/init_test.go=func TestInit_getUpgradePlugins(t *testing.T) {
command/init_test.go:   providerSource, close := newMockProviderSource(t, map[string][]string{
command/init_test.go:           ProviderSource:   providerSource,
command/init_test.go=func TestInit_getProviderMissing(t *testing.T) {
command/init_test.go:   providerSource, close := newMockProviderSource(t, map[string][]string{
command/init_test.go:           ProviderSource:   providerSource,
command/init_test.go=func TestInit_providerLockFile(t *testing.T) {
command/init_test.go:   providerSource, close := newMockProviderSource(t, map[string][]string{
command/init_test.go:           ProviderSource:   providerSource,
command/init_test.go=func TestInit_pluginDirReset(t *testing.T) {
command/init_test.go:   providerSource, close := newMockProviderSource(t, nil)
command/init_test.go:                   ProviderSource:   providerSource,
command/init_test.go:                   ProviderSource:   providerSource, // still empty
command/init_test.go=func TestInit_pluginDirProviders(t *testing.T) {
command/init_test.go:   providerSource, close := newMockProviderSource(t, nil)
command/init_test.go:           ProviderSource:   providerSource,
command/init_test.go:   if calls := providerSource.CallLog(); len(calls) > 0 {
command/init_test.go=func TestInit_pluginDirProvidersDoesNotGet(t *testing.T) {
command/init_test.go:   providerSource, close := newMockProviderSource(t, map[string][]string{
command/init_test.go:           ProviderSource:   providerSource,
command/init_test.go:   if calls := providerSource.CallLog(); len(calls) > 0 {
command/init_test.go=func TestInit_pluginDirWithBuiltIn(t *testing.T) {
command/init_test.go:   providerSource, close := newMockProviderSource(t, nil)
command/init_test.go:           ProviderSource:   providerSource,
command/init_test.go=func TestInit_invalidBuiltInProviders(t *testing.T) {
command/init_test.go:   providerSource, close := newMockProviderSource(t, nil)
command/init_test.go:           ProviderSource:   providerSource,
command/providers_schema_test.go=func TestProvidersSchema_output(t *testing.T) {
command/providers_schema_test.go:                       providerSource, close := newMockProviderSource(t, map[string][]string{
command/providers_schema_test.go:                               ProviderSource:   providerSource,
command/providers_test.go=func TestProviders_modules(t *testing.T) {
command/providers_test.go:      providerSource, close := newMockProviderSource(t, map[string][]string{
command/providers_test.go:              ProviderSource:   providerSource,
command/show_test.go=func TestShow_json_output(t *testing.T) {
command/show_test.go:                   providerSource, close := newMockProviderSource(t, map[string][]string{
command/show_test.go:                           ProviderSource:   providerSource,
command/show_test.go=func TestShow_json_output_state(t *testing.T) {
command/show_test.go:                   providerSource, close := newMockProviderSource(t, map[string][]string{
command/show_test.go:                           ProviderSource:   providerSource,
main.go=func wrappedMain() int {
main.go:        providerSrc, diags := providerSource(config.ProviderInstallation, services)
provider_source.go=import (
provider_source.go:// providerSource constructs a provider source based on a combination of the
provider_source.go:func providerSource(configs []*cliconfig.ProviderInstallation, services *disco.Disco) (getproviders.Source, tfdiags.Diagnostics) {
provider_source.go=func explicitProviderSource(config *cliconfig.ProviderInstallation, services *disco.Disco) (getproviders.Source, tfdiags.Diagnostics) {
provider_source.go:             source, moreDiags := providerSourceForCLIConfigLocation(methodConfig.Location, services)
provider_source.go=func implicitProviderSource(services *disco.Disco) getproviders.Source {
provider_source.go:func providerSourceForCLIConfigLocation(loc cliconfig.ProviderInstallationLocation, services *disco.Disco) (getproviders.Source, tfdiags.Diagnostics) {

## 6. git log -SglobalPluginDirs --oneline

35a058fb3 main: configure credentials from the CLI config file
c0b176109 prevent log output during init
8364383c3 Push plugin discovery down into command package


## 7.	git log -SsynchronizedWriters --pretty=format:"%an"

Martin Atkins
