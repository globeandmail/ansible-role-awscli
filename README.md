# ansible-role-awscli

##### Ansible role to install &amp; manage AWS CLI runtime / user configs

Default Variables:

    awscli_region: "us-east-1"
    awscli_users: []

Available Variables:

    awscli_users:
    - name: EXISTING_USER
      profiles:
      - name: "PROFILE_NAME"
        region: "REGION" (default awscli_region)
        output: "OUTPUT_TYPE" (default json)
        access: "ACCESS_KEY_ID" (ideally ansible-vault)
        secret: "SECRET_ACCESS_KEY" (ideally ansible-vault)