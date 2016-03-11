# ansible-azure-custom-image
A sample Ansible (1.9) runbook for creating an Azure custom image to deploy to multiple storage accounts

# Running the Playbook

To run the sample playbook, enter the variables for your Azure account in [run_capture.yml](./run_capture.yml) and run:

```bash
# hosts file is empty, intentionally
ansible-playbook -i hosts run_capture.yml
```

The playbook will deploy a VM within a new resource group, deprovision all the user information, capture the VM image and copy the image into the provided storage accounts.
