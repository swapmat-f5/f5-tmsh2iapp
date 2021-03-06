![tmsh2iapp main diagram](https://github.com/f5devcentral/f5-tmsh2iapp/wiki/images/tmsh2iapp_main_diagram.png)

# f5-tmsh2iapp
tmsh2iapp is an iApp generator using an existing configuration, also generates Ansible templates, 
Heat plugins and iWorkflow JSON files to deploy them.

The purpose of this project is to make as easy as possible deploying services in the F5, 
automate and orchestrate them with third party SDN/NFV/Automation/Orchestration products.

One of the goals of the tool is that it's use is as simply as possible: iApp development knowlege is **not required**
but some fluency in tmsh syntax is recommended.

# Main characteristics of tmsh2iapp

* Allows creating an iApp using a **declarative** tmsh-like syntax (these are called .t2i files)
* Baseline .t2i files can be created easily with the BIG-IP GUI
* Helps deploying the iApp by creating sample Ansible playbooks, Heat templates and iWorkflow JSON files
* It can be used in any computer with perl installed -- including the BIG-IP
* It is not BIG-IP version specific but it is being tested with BIG-IP 11.6-13.0
* Supports LTM policies
* It has been used with LTM, AFM and PEM modules. ASM support is in the works.
* It allows importing (from external files) the following configuration objects:
    * apache-ssl-cert          SSL certificates management
    * browser-capabilities-db  browser capabilities DB file management
    * dashboard-viewset
    * data-group               External Data Group files management
    * device-capabilities-db   Device capabilities DB file management
    * external-monitor         External Monitor files management
    * ifile                    iFile files management
    * lwtunneltbl              LW4o6 table files management
    * ssl-cert                 SSL certificates management
    * ssl-crl                  SSL CRL files management
    * ssl-csr                  SSL Certificate Signing Request
    * ssl-key                  SSL certificate keys management


# Using tmsh2iapp

**Please refer to ![project's wiki page](https://github.com/f5devcentral/f5-tmsh2iapp/wiki/) for documentation, examples and guidelines of use.**

This tool is not supported by F5 support. If you find an issue, we would love to hear about it. Please let us know by [filling an issue](https://github.com/f5devcentral/f5-tmsh2iapp/issues) in this repository. Tell us as much as you can about what you found, how you found it, your environment, etc.. We also welcome you to file feature requests as issues.

Please note again that this tool is released to the community is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.

