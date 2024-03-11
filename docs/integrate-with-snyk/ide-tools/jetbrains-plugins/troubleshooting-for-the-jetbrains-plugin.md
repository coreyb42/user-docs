# Troubleshooting for the JetBrains plugin

To obtain plugin logs, navigate to **Help** > **Show Log in Finder** (Mac) or **Show Log in Explorer** (Windows).

You can find more help on locating logs in [the IntelliJ support article](https://intellij-support.jetbrains.com/hc/en-us/articles/207241085-Locating-IDE-log-files).

## Trusted root certificates issues

Please refer to [JetBrains documentation](https://www.jetbrains.com/help/idea/ssl-certificates.html) on how IDE resolves custom certificates and how to import them, in case plugin experiences any network failures due to incorrect configuration.

## Running on a remote IDE

If you are running your IDE remotely and using the Jetbrains Client, you must:

* install the plugin as a **host** plugin, not a client plugin
* if the authentication process does not work, visit your Snyk account page and retrieve your account token
* input the account token into Settings -> Tools -> Snyk -> Token
