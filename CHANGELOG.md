## 0.17.0

- Add encrypt-file command & decrypt feature for Lambda function [#62][]
- Bigfix: Fix error when import lamvery in function [#62][]

## 0.16.0

- Add `generate` command [#61][]
  - Generate the skeleton function

## 0.15.3

- Pull request [#60][]: Integrate API Gateway without api-id option([@koppeft][])

## 0.15.2

- Pull request [#58][]: Adding api and hook config to default excludes([@mathom][])

## 0.15.1

- Add `no_integrate` option to api command [#56][]

## 0.15.0

- API Gateway integration (beta) [#55][] [#46][]

## 0.14.1

- Bugfix: `init` command fails on root directory [#54][]

## 0.14.0

- Change the command `archive` to `build` [#53][]
- Add build hooks [#36][] [#53][]

## 0.13.0

- Add `-e`,`--env` option to `archive` and `deploy` command [#52][]
  - Pass some environment variables that are not encrypted [#50][]

## 0.12.4

- Bugfix: `init` command failure [#51][]

## 0.12.3

- Bugfix: The permission is not given to the alias [#48][]

## 0.12.2

- Improvement and bugfix for the feature of CloudWatch Events [#48][]
  - Change the format of the event configuration file (Backward compatible)
  - Use ARN of the alias to the event targets (Previously, It was used `$LATEST` by default)

## 0.12.1

- Allow empty setting to `description`,`timeout`,`mamory_size` [#44][]
  - Bugfix: deploy fails on empty description [#43][]

## 0.12.0

- Add VPC configuration [#42][]
  - You can now configure a Lambda function to access resources in your VPC!!  
    http://aws.amazon.com/releasenotes/8144743194161467

## 0.11.2

- Bugfix [#41][]

## 0.11.1

- Add `-t`, `--target` option to `set-alias` commnad [#40][]  
  - The alias of the version that is targeted for setting alias

## 0.11.0

- Add `logs` commnad [#39][]

## 0.10.2

- Bugfix: `init` command fail in the case that the configuration file does not exist. [#37][]

## 0.10.1

- Add KMS support for Node.js [#35][]

## 0.10.0

- Split the configuration file [#33][]
- Bugfix

## 0.9.0

- Pull request [#28][]: Single file upload support ([@ijin][])
- Adjust some outputs
- Add `rollback` command [#29][]
  - Remove `configuration.alias` from the configuration file
  - Add `default_alias` to the configuration file
  - Add `versioning` to the configuration file

## 0.8.2

- Pull request [#27][]: Adjust final capacity depending on publishing lambda function or not ([@ijin][])

## 0.8.1

- Exclusion list support [#26][]

## 0.8.0

- Add invoke command [#18][] [#25][]
- Allow archiving without `virtualenv` [#23][] [#25][]
- Initial support `node.js` runtime [#23][] [#25][]
- Bugfix [#24][] [#25][]

## 0.7.0

- Support CloudWatch Events [#22][] [#3][]

## 0.6.0

- Change the secret file format YAML -> JSON
- Reduce capacity of the archive
- Bugfix

## 0.5.2

- Bugfix

## 0.5.1

- Bugfix

## 0.5.0

- Add `-l`,`--no-libs` option to archive without all libraries [#20][] [#21][]
- Calculate and print the function's usage capacity [#19][] [#21][]

## 0.4.0

- Change configuration file option `secret: key` -> `secret: key_id` [#17][]
- Simplify importing of `lamvery.secret` [#17][]
- Lost jinja2 descriptor when call `encrypt` command with `-s` option [#17][]

## 0.3.3

- Exclude bin directory form archive(Reduce size of the archive file)

## 0.3.2

- Add some files to list of exclude from the archive

## 0.3.1

- Bugfix: Duplicate output on `deploy`

## 0.3.0

- Support jinja2 template in configuration file [#15][]

## 0.2.0

- Change default name of the configuration file to '.lamvery.yml'
- Change format of the configuration file (See: [README](https://github.com/marcy-terui/lamvery/blob/master/README.md#setup))
- Support passing some confidential informations using KMS [#8][]
- Add `encrypt` command
- Add `decrypt` command
- Adjust all outputs

## 0.1.0

- Support `profile` specification [#6][] [#10][]
- Change `publish` to command-line argument [#9][]

## 0.0.6

- Collect help messages

## 0.0.5

- Add `alias` option [#1][] [#7][]

## 0.0.4

- Add `region` option
- Refactoring

## 0.0.3

- Bugfix

## 0.0.2

- Bugfix

## 0.0.1

- Initial release

<!--- The following link definition list is generated by PimpMyChangelog --->
[#1]: https://github.com/marcy-terui/lamvery/issues/1
[#3]: https://github.com/marcy-terui/lamvery/issues/3
[#6]: https://github.com/marcy-terui/lamvery/issues/6
[#7]: https://github.com/marcy-terui/lamvery/issues/7
[#8]: https://github.com/marcy-terui/lamvery/issues/8
[#9]: https://github.com/marcy-terui/lamvery/issues/9
[#10]: https://github.com/marcy-terui/lamvery/issues/10
[#15]: https://github.com/marcy-terui/lamvery/issues/15
[#17]: https://github.com/marcy-terui/lamvery/issues/17
[#18]: https://github.com/marcy-terui/lamvery/issues/18
[#19]: https://github.com/marcy-terui/lamvery/issues/19
[#20]: https://github.com/marcy-terui/lamvery/issues/20
[#21]: https://github.com/marcy-terui/lamvery/issues/21
[#22]: https://github.com/marcy-terui/lamvery/issues/22
[#23]: https://github.com/marcy-terui/lamvery/issues/23
[#24]: https://github.com/marcy-terui/lamvery/issues/24
[#25]: https://github.com/marcy-terui/lamvery/issues/25
[#26]: https://github.com/marcy-terui/lamvery/issues/26
[#27]: https://github.com/marcy-terui/lamvery/issues/27
[#28]: https://github.com/marcy-terui/lamvery/issues/28
[#29]: https://github.com/marcy-terui/lamvery/issues/29
[#33]: https://github.com/marcy-terui/lamvery/issues/33
[#35]: https://github.com/marcy-terui/lamvery/issues/35
[#36]: https://github.com/marcy-terui/lamvery/issues/36
[#37]: https://github.com/marcy-terui/lamvery/issues/37
[#39]: https://github.com/marcy-terui/lamvery/issues/39
[#40]: https://github.com/marcy-terui/lamvery/issues/40
[#41]: https://github.com/marcy-terui/lamvery/issues/41
[#42]: https://github.com/marcy-terui/lamvery/issues/42
[#43]: https://github.com/marcy-terui/lamvery/issues/43
[#44]: https://github.com/marcy-terui/lamvery/issues/44
[#46]: https://github.com/marcy-terui/lamvery/issues/46
[#48]: https://github.com/marcy-terui/lamvery/issues/48
[#50]: https://github.com/marcy-terui/lamvery/issues/50
[#51]: https://github.com/marcy-terui/lamvery/issues/51
[#52]: https://github.com/marcy-terui/lamvery/issues/52
[#53]: https://github.com/marcy-terui/lamvery/issues/53
[#54]: https://github.com/marcy-terui/lamvery/issues/54
[#55]: https://github.com/marcy-terui/lamvery/issues/55
[#56]: https://github.com/marcy-terui/lamvery/issues/56
[#58]: https://github.com/marcy-terui/lamvery/issues/58
[#60]: https://github.com/marcy-terui/lamvery/issues/60
[#61]: https://github.com/marcy-terui/lamvery/issues/61
[@ijin]: https://github.com/ijin
[@koppeft]: https://github.com/koppeft
[@mathom]: https://github.com/mathom
