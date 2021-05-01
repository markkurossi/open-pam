# open-pam
Open Privileged Access Management (PAM)

<pre style="font-family: menlo, consolas, monospace; font-size: 10pt;">
                                 ┌───────────────────┐
                             ┌───┤     SSH Agent     │
                             │   └───────────────────┘
            ┌────────────┐   │
            │            │   │   ┌───────────────────┐
            │            │   ├───┤     PAM Shell     │
            │            │   │   └───────────────────┘
            │ Authorizer │   │
┌───────┐   │            │   │   ╭───────────────────╮
│ Vault ├───┤            ├───┼───┤ <a href="https://github.com/markkurossi/pkcs11─provider">PKCS #11 Provider</a> │
└───────┘   │  ╭─────╮   │   │   ╰───────────────────╯
            │  │ OPA │   │   │
            │  ╰─────╯   │   │   ┌───────────────────┐
            │            │   ├───┤      PAM RDP      │
            │            │   │   └───────────────────┘
            └────────────┘   │
                             │   ╭───────────────────╮
                             └───┤  <a href="https://github.com/markkurossi/pam─cert">PAM Certificate</a>  │
                                 ╰───────────────────╯
</pre>
