# testing


| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:--------:|
| events_lambda_quicksight_enabled | Should QuickSight Lambda be deployed? | `bool` | `"true"` | yes |
| quicksight_rules_enabled | Should QuickSight event rule be enabled? | `bool` | `"true"` | yes |
| quicksight_eventbridge_bus_name | Quicksight eventbridge bus name to which AWS Tags rule should be attached. | `string` | `"default"` | yes |
| quicksight_user_registration_events_lambda | Lambda funciton triggered by quicksight event source | `string` | `"dcs-aws-events-quicksight-user-register"` | yes |
| events_quicksight_user_registration | event rule to capture quicksight user registration | `string` | `"capture-aws-quicksight-user-registration"` | yes |
| events_lambda_quicksight_kms_key_alias | Alias for evemts,quicksight,lambda KMS key | `string` | "`dcs-aws-events-lambda-quicksight-kms`" |
| quicksight_group | Tag of the quicksight group | `string` | `""` | yes |
| environment_tag | Tag of the environment the components is associated with | `string` | `"dev"` | yes |
| service_tag | Tag of the service the components is associated with | `string` | `"DCS-Security"` | yes |
| team_tag | Tag of the team that manages the solution | `string` | `"Atos-CES-AWS`" | yes |
| pipeline_tag | GitHub action pipeline ID information, auto generated.  Where testing locally or in break glass situations use local, time and date instead, e.g. local-1805-19022021 | `string` | `"pipeline"` | yes |
| tags | A map of tags to add to IAM role resources | `map(string)` | `"{ }"` | yes |
