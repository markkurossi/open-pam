# open-pam
Open Privileged Access Management (PAM)

![Open PAM](open-pam.png)

<pre style="font-family: menlo, consolas, monospace; font-size: 10pt;">
                                 ┌───────────────────┐
            ┌────────────┐   ┌───┤     SSH Agent     │
            │            │   │   └───────────────────┘
            │            │   │
            │            │   │   ┌───────────────────┐
            │ Authorizer │   ├───┤     PAM Shell     │
┌───────┐   │            │   │   └───────────────────┘
│ Vault ├───┤            ├───┤
└───────┘   │  ┌─────┐   │   │   ┌───────────────────┐
            │  │ OPA │   │   ├───┤ <a href="https://github.com/markkurossi/pkcs11-provider">PKCS #11 Provider</a> │
            │  └─────┘   │   │   └───────────────────┘
            │            │   │
            │            │   │   ┌───────────────────┐
            └────────────┘   ├───┤      PAM RDP      │
                             │   └───────────────────┘
                             │
                             │   ┌───────────────────┐
                             └───┤  PAM Certificate  │
                                 └───────────────────┘
</pre>
