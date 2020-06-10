# Cannot_change_type_due_to_existing_data

```
$ sfdx force:org:create -f config/project-scratch-def.json -a error-test --durationdays 1 --setdefaultusername -v TsubaisoDevHub
$ sfdx force:source:push -u error-test
```

Results

```
goldmac:error-test sanya$ sfdx force:org:create -f config/project-scratch-def.json -a error-test --durationdays 1 --setdefaultusername -v TsubaisoDevHub
Successfully created scratch org: 00D1m0000008enbEAA, username: test-03egis5av6av@example.com
goldmac:error-test sanya$ sfdx force:source:push -u error-test
Job ID | 0Af1m000003ah9BCAQ
SOURCE PROGRESS | ██████████████████████████████████████░░ | 20/21 Components
TYPE   PROJECT PATH                                                                                       PROBLEM
─────  ─────────────────────────────────────────────────────────────────────────────────────────────────  ────────────────────────────────────────────────
Error  force-app/main/default/objects/tb_Cost__c/fields/tb_GoodsInProcessAmountWithTax__c.field-meta.xml  Cannot change type due to existing data (161:13)
ERROR running force:source:push:  Push failed.
```
