# Setup

* Install Virtual Machine Manager and QEMU

* The [Windows Server 2022 Evaluation image](https://go.microsoft.com/fwlink/p/?LinkID=2195280&clcid=0x409&culture=en-us&country=US) is already referenced by the customized Packer script, added here for reference.

* Install Packer

# Run

* `mkdir -p logs`

* `packer build -on-error=ask -timestamp-ui images/windows/templates/build.windows-2022.pkr.hcl  | tee logs/$(date +"%Y%m%dT%H%M%S").log`
