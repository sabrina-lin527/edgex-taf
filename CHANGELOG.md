
<a name="EdgeX Test Automation (found in edgex-taf) Changelog"></a>
## EdgeX Test Automation
[Github repository](https://github.com/edgexfoundry/edgex-taf)

## [4.0.2] - 2026-05-31

### ✨ Features 
- Implement tag test for DeviceResource and DeviceCommand ([#12167d9](https://github.com/edgexfoundry/edgex-taf/commits/12167d9))
- Add test scenarios for tags and asynchronous `edgex-private` operations ([#18d0163](https://github.com/edgexfoundry/edgex-taf/commits/18d0163))
- Implement integration test for external JWT authentication ([#7fee600](https://github.com/edgexfoundry/edgex-taf/commits/7fee600))
- Implement integration tests for maximum device and resource configurations ([#e1d013a](https://github.com/edgexfoundry/edgex-taf/commits/e1d013a))
- Implement bidirectional `DataTransform` integration tests with Modbus ([#6adde39](https://github.com/edgexfoundry/edgex-taf/commits/6adde39))
- Add integration test scenarios for device and resource capacity limits ([#ab76b0d](https://github.com/edgexfoundry/edgex-taf/commits/ab76b0d))
- Implement integration tests for device up/down detection ([#842394e](https://github.com/edgexfoundry/edgex-taf/commits/842394e))
- Add performance test script ([#d561fa8](https://github.com/edgexfoundry/edgex-taf/commits/d561fa8))
- Add tests for device parent feature ([#942](https://github.com/edgexfoundry/edgex-taf/issues/942)) ([#15a3c13](https://github.com/edgexfoundry/edgex-taf/commits/15a3c13))
- Update Odessa branch image size on main branch ([#948](https://github.com/edgexfoundry/edgex-taf/issues/948)) ([#da0edd0](https://github.com/edgexfoundry/edgex-taf/commits/da0edd0))

### 🐛 Bug Fixes 
- Update the incorrect field name in `trigger_data.json` and restrict `SchedulerJobTriggerPOST001` to only allow manual-triggered jobs during testing ([#776d767](https://github.com/edgexfoundry/edgex-taf/commits/776d767))
- Fix missing `core-keeper` executable footprint data in the performance report ([#628f338](https://github.com/edgexfoundry/edgex-taf/commits/628f338))
- Update keyword to fix error after upgrading Python libraries and download `requirements.txt` instead of using the local file ([#bc4fffa](https://github.com/edgexfoundry/edgex-taf/commits/bc4fffa))
- Replace `mqtt-broker` with `mqtt-taf-broker` on performance test ([#707c593](https://github.com/edgexfoundry/edgex-taf/commits/707c593))

### 👷 Build 
- Apply `taf-common` v1 changes to command options and variable names ([#952](https://github.com/edgexfoundry/edgex-taf/issues/952)) ([#31cae56](https://github.com/edgexfoundry/edgex-taf/commits/31cae56))
- Migrate `paho-mqtt` from v1 to v2 ([#950](https://github.com/edgexfoundry/edgex-taf/issues/950)) ([#71d12e1](https://github.com/edgexfoundry/edgex-taf/commits/71d12e1))



## [v2.0.0] Ireland - 2021-06-30  (Not Compatible with 1.x releases)

### Features ✨
- Add changing `device-modbus:` to `edgex-device-modbus:` and setting URL to master ([#6610122](https://github.com/edgexfoundry/edgex-taf/commits/6610122))
- Fixed TAF Perf to proply also pull the standard compose file ([#8d68d5e](https://github.com/edgexfoundry/edgex-taf/commits/8d68d5e))
- Switch to use edgex-mqtt-broker and removed EXPORT_HOST_PLACE_HOLDER replacement ([#405d454](https://github.com/edgexfoundry/edgex-taf/commits/405d454))
- Changed output of docker-compose-end-mqtt.yaml to docker-compose-mqtt.yaml ([#dfbd838](https://github.com/edgexfoundry/edgex-taf/commits/dfbd838))
- Removed references to the ${ARCH}.env files ([#6f07626](https://github.com/edgexfoundry/edgex-taf/commits/6f07626))
- Add Modbus scalability testing ([#b80dbeb](https://github.com/edgexfoundry/edgex-taf/commits/b80dbeb))
### Bug Fixes 🐛
- Update service key name in token path to new name ([#f998962](https://github.com/edgexfoundry/edgex-taf/commits/f998962))
- Update gateway token generation ([#038becc](https://github.com/edgexfoundry/edgex-taf/commits/038becc))
### Code Refactoring ♻
- Update container names for those recently changed ([#b2ebc50](https://github.com/edgexfoundry/edgex-taf/commits/b2ebc50))
- Update the route names to the new service key based names ([#0410181](https://github.com/edgexfoundry/edgex-taf/commits/0410181))
- Update to use new port assignments ([#c750538](https://github.com/edgexfoundry/edgex-taf/commits/c750538))
- Additional changes from PR comments ([#c8c4eb1](https://github.com/edgexfoundry/edgex-taf/commits/c8c4eb1))
- Update for service key name changes to remove edgex- prefix ([#598cda5](https://github.com/edgexfoundry/edgex-taf/commits/598cda5))
- Change delpoy-edgex.sh to deplaoy all security services together ([#8b12dd4](https://github.com/edgexfoundry/edgex-taf/commits/8b12dd4))
- Change gateway port to 8100 ([#c60127f](https://github.com/edgexfoundry/edgex-taf/commits/c60127f))
- Update App Service tests for change in service key ([#faf4730](https://github.com/edgexfoundry/edgex-taf/commits/faf4730))
- Switch to 2.0 Consul path ([#df0134c](https://github.com/edgexfoundry/edgex-taf/commits/df0134c))
- Update docker scripts to pull compose files from new location ([#11b0e2c](https://github.com/edgexfoundry/edgex-taf/commits/11b0e2c))
- Rename SetOutputData to SetResponseData ([#4af9c12](https://github.com/edgexfoundry/edgex-taf/commits/4af9c12))
- App Service Trigger tests for function configuration changes ([#ce9915b](https://github.com/edgexfoundry/edgex-taf/commits/ce9915b))
- Update scripts to pull compose files from edgex-compose repo ([#f25c686](https://github.com/edgexfoundry/edgex-taf/commits/f25c686))
- Use new nightly build TAF compose files ([#186834e](https://github.com/edgexfoundry/edgex-taf/commits/186834e))
### Documentation 📖
- Add badges to readme ([#1f5bfad](https://github.com/edgexfoundry/edgex-taf/commits/1f5bfad))
### Reverts
- Add scheduler tests to SmokeTest for kong issue
- refactor: Change gateway port to 8100
- Change image url to use dockerhub hanoi release

<a name="v1.3.0"></a>
## [v1.3.0] - 2020-11-20
### Bug Fixes 🐛
- Fixed links to nightly-build compose files to point to edgexfoundry master ([#a5ef11f](https://github.com/edgexfoundry/edgex-taf/commits/a5ef11f))
### Code Refactoring ♻
- Adjust URL path to base compose file now under new compose-generator ([#ec3e15f](https://github.com/edgexfoundry/edgex-taf/commits/ec3e15f))
- renamed existing common.env to common-taf.env to avoid name conflict ([#bb20039](https://github.com/edgexfoundry/edgex-taf/commits/bb20039))
- added changing the database service name to `database` in previous compose files. ([#c5d729e](https://github.com/edgexfoundry/edgex-taf/commits/c5d729e))
- Replace `redis` service name with `database` so deploy works ([#40d51a5](https://github.com/edgexfoundry/edgex-taf/commits/40d51a5))
- Updated scripts to use curl and pull from new `source` folder. ([#84241da](https://github.com/edgexfoundry/edgex-taf/commits/84241da))
- Fixed typo if "-arm64" ([#105a52f](https://github.com/edgexfoundry/edgex-taf/commits/105a52f))
- Updated get-compose-file-backward.sh to use base compose file from nightly-build ([#87a1ec1](https://github.com/edgexfoundry/edgex-taf/commits/87a1ec1))
- Update scripts to handle chnage to multi-file compose files. ([#b35cc52](https://github.com/edgexfoundry/edgex-taf/commits/b35cc52))
