# Comparing `tmp/dcentralab_qa_infra_automation-1.0.3.tar.gz` & `tmp/dcentralab_qa_infra_automation-1.0.4.tar.gz`

## Comparing `dcentralab_qa_infra_automation-1.0.3.tar` & `dcentralab_qa_infra_automation-1.0.4.tar`

### file list

```diff
@@ -1,52 +1,60 @@
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.3/.idea/.gitignore
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.3/.idea/misc.xml
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.3/.idea/modules.xml
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.3/.idea/packaging.iml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.3/.idea/vcs.xml
--rw-r--r--   0        0        0    10853 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.3/.idea/workspace.xml
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.3/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.3/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.3/src/dcentralab_qa_infra_automation/__init__.py
--rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.3/src/dcentralab_qa_infra_automation/data/read_data.py
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.3/src/dcentralab_qa_infra_automation/drivers/BraveDriver.py
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.3/src/dcentralab_qa_infra_automation/drivers/ChromeDriver.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.3/src/dcentralab_qa_infra_automation/drivers/HelperFunctions.py
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.3/src/dcentralab_qa_infra_automation/fixtures/CreateTargetDirectory.py
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.3/src/dcentralab_qa_infra_automation/fixtures/HtmlReports.py
--rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.3/src/dcentralab_qa_infra_automation/fixtures/InitGlobalParameters.py
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.3/src/dcentralab_qa_infra_automation/fixtures/Loggers.py
--rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.3/src/dcentralab_qa_infra_automation/fixtures/OpenSiteWithCRXExtension.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.3/src/dcentralab_qa_infra_automation/fixtures/ParameterInjection.py
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.3/src/dcentralab_qa_infra_automation/fixtures/ReportLoggers.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.3/src/dcentralab_qa_infra_automation/fixtures/Screenshot.py
--rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.3/src/dcentralab_qa_infra_automation/fixtures/SetupDriver.py
--rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.3/src/dcentralab_qa_infra_automation/infra/CustomEventListener.py
--rw-r--r--   0        0        0     6515 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.3/src/dcentralab_qa_infra_automation/pages/BasePage.py
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.3/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConfirmPage.py
--rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.3/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConfirmRequestPage.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.3/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConnectToWebsitePage.py
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.3/src/dcentralab_qa_infra_automation/pages/coinbasePages/CreatePasswordPage.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.3/src/dcentralab_qa_infra_automation/pages/coinbasePages/CreateWalletPage.py
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.3/src/dcentralab_qa_infra_automation/pages/coinbasePages/ImportWalletPage.py
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.3/src/dcentralab_qa_infra_automation/pages/coinbasePages/ReceiveCryptoToUsername.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.3/src/dcentralab_qa_infra_automation/pages/coinbasePages/UseAnExistingWalletPage.py
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.3/src/dcentralab_qa_infra_automation/pages/metamaskPages/ConfirmPage.py
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.3/src/dcentralab_qa_infra_automation/pages/metamaskPages/CongratulationsPage.py
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.3/src/dcentralab_qa_infra_automation/pages/metamaskPages/ConnectWithWalletPage.py
--rw-r--r--   0        0        0     4112 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.3/src/dcentralab_qa_infra_automation/pages/metamaskPages/ImportWalletPage.py
--rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.3/src/dcentralab_qa_infra_automation/pages/metamaskPages/ImproveMetamaskPage.py
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.3/src/dcentralab_qa_infra_automation/pages/metamaskPages/NewToMetamaskPage.py
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.3/src/dcentralab_qa_infra_automation/pages/metamaskPages/SwitchNetworkPage.py
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.3/src/dcentralab_qa_infra_automation/pages/metamaskPages/WalletConnectedHomePage.py
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.3/src/dcentralab_qa_infra_automation/pages/metamaskPages/WelcomeToMetamaskPage.py
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.3/src/dcentralab_qa_infra_automation/utils/HTTPMethods.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.3/src/dcentralab_qa_infra_automation/utils/WalletsActionsInterface.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.3/src/dcentralab_qa_infra_automation/utils/enum/HTTPStatusCodes.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.3/src/dcentralab_qa_infra_automation/utils/enum/NetworkTypes.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.3/src/dcentralab_qa_infra_automation/utils/enum/Wallets.py
--rw-r--r--   0        0        0     4870 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.3/src/dcentralab_qa_infra_automation/walletsActions/CoinbaseActions.py
--rw-r--r--   0        0        0     6121 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.3/src/dcentralab_qa_infra_automation/walletsActions/MetamaskActions.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.3/LICENSE
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.3/README.md
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.3/pyproject.toml
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/.idea/.gitignore
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/.idea/misc.xml
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/.idea/modules.xml
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/.idea/packaging.iml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/.idea/vcs.xml
+-rw-r--r--   0        0        0    11734 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/.idea/workspace.xml
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/__init__.py
+-rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/data/read_data.py
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/drivers/BraveDriver.py
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/drivers/ChromeDriver.py
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/drivers/HelperFunctions.py
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/fixtures/CreateTargetDirectory.py
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/fixtures/HtmlReports.py
+-rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/fixtures/InitGlobalParameters.py
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/fixtures/Loggers.py
+-rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/fixtures/OpenSiteWithCRXExtension.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/fixtures/ParameterInjection.py
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/fixtures/ReportLoggers.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/fixtures/Screenshot.py
+-rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/fixtures/SetupDriver.py
+-rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/infra/CustomEventListener.py
+-rw-r--r--   0        0        0     7209 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/BasePage.py
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConfirmPage.py
+-rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConfirmRequestPage.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConnectToWebsitePage.py
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/coinbasePages/CreatePasswordPage.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/coinbasePages/CreateWalletPage.py
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/coinbasePages/ImportWalletPage.py
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/coinbasePages/ReceiveCryptoToUsername.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/coinbasePages/UseAnExistingWalletPage.py
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/metamaskPages/ConfirmPage.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/metamaskPages/CongratulationsPage.py
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/metamaskPages/ConnectWithWalletPage.py
+-rw-r--r--   0        0        0     4112 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/metamaskPages/ImportWalletPage.py
+-rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/metamaskPages/ImproveMetamaskPage.py
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/metamaskPages/NewToMetamaskPage.py
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/metamaskPages/SwitchNetworkPage.py
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/metamaskPages/WalletConnectedHomePage.py
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/metamaskPages/WelcomeToMetamaskPage.py
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/namiPages/ConnectWalletPage.py
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/namiPages/CreateAccountPage.py
+-rw-r--r--   0        0        0     4700 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/namiPages/ImportSeedPhrasePage.py
+-rw-r--r--   0        0        0     2223 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/namiPages/NamiBasePage.py
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/namiPages/SignPage.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/namiPages/SuccessfullyCreatedWalletPage.py
+-rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/namiPages/WelcomePage.py
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/utils/HTTPMethods.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/utils/WalletsActionsInterface.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/utils/enum/HTTPStatusCodes.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/utils/enum/NetworkTypes.py
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/utils/enum/Wallets.py
+-rw-r--r--   0        0        0     4945 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/walletsActions/CoinbaseActions.py
+-rw-r--r--   0        0        0     6196 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/walletsActions/MetamaskActions.py
+-rw-r--r--   0        0        0     6821 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/walletsActions/NamiActions.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/LICENSE
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/README.md
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/PKG-INFO
```

### Comparing `dcentralab_qa_infra_automation-1.0.3/.idea/workspace.xml` & `dcentralab_qa_infra_automation-1.0.4/.idea/workspace.xml`

 * *Files 5% similar despite different names*

#### Comparing `dcentralab_qa_infra_automation-1.0.3/.idea/workspace.xml` & `dcentralab_qa_infra_automation-1.0.4/.idea/workspace.xml`

```diff
@@ -21,22 +21,25 @@
       <change afterPath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/pages/metamaskPages/ImproveMetamaskPage.py" afterDir="false"/>
       <change afterPath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/pages/metamaskPages/NewToMetamaskPage.py" afterDir="false"/>
       <change afterPath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/pages/metamaskPages/SwitchNetworkPage.py" afterDir="false"/>
       <change afterPath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/pages/metamaskPages/WalletConnectedHomePage.py" afterDir="false"/>
       <change afterPath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/pages/metamaskPages/WelcomeToMetamaskPage.py" afterDir="false"/>
       <change afterPath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/walletsActions/CoinbaseActions.py" afterDir="false"/>
       <change afterPath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/walletsActions/MetamaskActions.py" afterDir="false"/>
+      <change afterPath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/walletsActions/NamiActions.py" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/pyproject.toml" beforeDir="false" afterPath="$PROJECT_DIR$/pyproject.toml" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/drivers/BraveDriver.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/drivers/BraveDriver.py" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/drivers/ChromeDriver.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/drivers/ChromeDriver.py" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/fixtures/InitGlobalParameters.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/fixtures/InitGlobalParameters.py" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/fixtures/Loggers.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/fixtures/Loggers.py" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/fixtures/OpenSiteWithCRXExtension.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/fixtures/OpenSiteWithCRXExtension.py" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/fixtures/SetupDriver.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/fixtures/SetupDriver.py" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/fixtures/SetupDriverWithMetamaskExtension.py" beforeDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/utils/WalletsActionsInterface.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/utils/WalletsActionsInterface.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/utils/enum/Wallets.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/utils/enum/Wallets.py" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/src/seleniumPythonFramework_VeriSoft/__init__.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/drivers/HelperFunctions.py" afterDir="false"/>
     </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
@@ -155,11 +158,16 @@
     <breakpoint-manager>
       <breakpoints>
         <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
           <url>file://$PROJECT_DIR$/src/dcentralab_qa_infra_automation/fixtures/InitGlobalParameters.py</url>
           <line>23</line>
           <option name="timeStamp" value="5"/>
         </line-breakpoint>
+        <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
+          <url>file://$PROJECT_DIR$/src/dcentralab_qa_infra_automation/fixtures/InitGlobalParameters.py</url>
+          <line>32</line>
+          <option name="timeStamp" value="6"/>
+        </line-breakpoint>
       </breakpoints>
     </breakpoint-manager>
   </component>
 </project>
```

### Comparing `dcentralab_qa_infra_automation-1.0.3/.idea/inspectionProfiles/Project_Default.xml` & `dcentralab_qa_infra_automation-1.0.4/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.3/src/dcentralab_qa_infra_automation/data/read_data.py` & `dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/data/read_data.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.3/src/dcentralab_qa_infra_automation/drivers/BraveDriver.py` & `dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/drivers/BraveDriver.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.3/src/dcentralab_qa_infra_automation/drivers/ChromeDriver.py` & `dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/drivers/ChromeDriver.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.3/src/dcentralab_qa_infra_automation/drivers/HelperFunctions.py` & `dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/drivers/HelperFunctions.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,9 +15,11 @@
     """
     add_extension = None
     # In metamask wallet type
     if pytest.data_driven.get("wallet_type") == 'MetaMask':
         add_extension = pytest.user_dir + pytest.properties.get("metamask.extension.crx")
     elif pytest.data_driven.get("wallet_type") == 'Coinbase':
         add_extension = pytest.user_dir + pytest.properties.get("coinbase.extension.crx")
+    elif pytest.data_driven.get("wallet_type") == 'Nami':
+        add_extension = pytest.user_dir + pytest.properties.get("nami.extension.crx")
 
     return add_extension
```

### Comparing `dcentralab_qa_infra_automation-1.0.3/src/dcentralab_qa_infra_automation/fixtures/CreateTargetDirectory.py` & `dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/fixtures/CreateTargetDirectory.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.3/src/dcentralab_qa_infra_automation/fixtures/HtmlReports.py` & `dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/fixtures/HtmlReports.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.3/src/dcentralab_qa_infra_automation/fixtures/InitGlobalParameters.py` & `dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/fixtures/InitGlobalParameters.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.3/src/dcentralab_qa_infra_automation/fixtures/Loggers.py` & `dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/fixtures/Loggers.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.3/src/dcentralab_qa_infra_automation/fixtures/OpenSiteWithCRXExtension.py` & `dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/fixtures/OpenSiteWithCRXExtension.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.3/src/dcentralab_qa_infra_automation/fixtures/ParameterInjection.py` & `dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/fixtures/ParameterInjection.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.3/src/dcentralab_qa_infra_automation/fixtures/ReportLoggers.py` & `dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/fixtures/ReportLoggers.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.3/src/dcentralab_qa_infra_automation/fixtures/Screenshot.py` & `dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/fixtures/Screenshot.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.3/src/dcentralab_qa_infra_automation/fixtures/SetupDriver.py` & `dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/fixtures/SetupDriver.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.3/src/dcentralab_qa_infra_automation/infra/CustomEventListener.py` & `dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/infra/CustomEventListener.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.3/src/dcentralab_qa_infra_automation/pages/BasePage.py` & `dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/BasePage.py`

 * *Files 12% similar despite different names*

```diff
@@ -95,25 +95,40 @@
          Performs text entry of the passed in text, in a web element whose locator is passed to it
          :param element_name - current element name
          :param by_locator - current locator
          :param text - test to insert
         """
 
         pytest.logger.info("insert value: " + text + " into " + element_name + " element")
-        return WebDriverWait(self.driver, self.timeout).until(EC.visibility_of_element_located(by_locator)).send_keys(text)
+        return WebDriverWait(self.driver, self.timeout).until(EC.visibility_of_element_located(by_locator)).send_keys(
+            text)
+
+    def enter_text_on_specific_list_item(self, element_name, by_locator, index, text):
+        """
+         Performs text entry of the passed in text, in a web element whose locator is passed to it
+         :param element_name - current element name
+         :param by_locator - current locator
+         :param index - current index
+         :param text - test to insert
+        """
+
+        pytest.logger.info("insert value: " + text + " into " + element_name + " in index " + str(index) + " element")
+        return WebDriverWait(self.driver, self.timeout).until(EC.visibility_of_all_elements_located(by_locator))[
+            index].send_keys(text)
 
     def upload_file(self, element_name, by_locator, file_path):
         """
         Performs choose file in input with type file, in a web element whose locator and file path are passed to it
         :param element_name - current element name
         :param by_locator - current locator to click on
         :param file_path:
         """
         pytest.logger.info("upload file: " + file_path + " into " + element_name + " element")
-        return WebDriverWait(self.driver, self.timeout).until(EC.visibility_of_element_located(by_locator)).send_keys(file_path)
+        return WebDriverWait(self.driver, self.timeout).until(EC.visibility_of_element_located(by_locator)).send_keys(
+            file_path)
 
     def get_text(self, element_name, by_locator):
         """
         Performs get text of web element whose locator is passed to it
         :param by_locator - current locator
         :param element_name: - current element
         :return current element text
```

### Comparing `dcentralab_qa_infra_automation-1.0.3/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConfirmPage.py` & `dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConfirmPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.3/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConfirmRequestPage.py` & `dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConfirmRequestPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.3/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConnectToWebsitePage.py` & `dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConnectToWebsitePage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.3/src/dcentralab_qa_infra_automation/pages/coinbasePages/CreatePasswordPage.py` & `dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/coinbasePages/CreatePasswordPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.3/src/dcentralab_qa_infra_automation/pages/coinbasePages/CreateWalletPage.py` & `dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/coinbasePages/CreateWalletPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.3/src/dcentralab_qa_infra_automation/pages/coinbasePages/ImportWalletPage.py` & `dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/coinbasePages/ImportWalletPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.3/src/dcentralab_qa_infra_automation/pages/coinbasePages/ReceiveCryptoToUsername.py` & `dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/coinbasePages/ReceiveCryptoToUsername.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.3/src/dcentralab_qa_infra_automation/pages/coinbasePages/UseAnExistingWalletPage.py` & `dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/coinbasePages/UseAnExistingWalletPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.3/src/dcentralab_qa_infra_automation/pages/metamaskPages/ConfirmPage.py` & `dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/metamaskPages/ConfirmPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.3/src/dcentralab_qa_infra_automation/pages/metamaskPages/CongratulationsPage.py` & `dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/metamaskPages/CongratulationsPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.3/src/dcentralab_qa_infra_automation/pages/metamaskPages/ConnectWithWalletPage.py` & `dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/metamaskPages/ConnectWithWalletPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.3/src/dcentralab_qa_infra_automation/pages/metamaskPages/ImportWalletPage.py` & `dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/metamaskPages/ImportWalletPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.3/src/dcentralab_qa_infra_automation/pages/metamaskPages/ImproveMetamaskPage.py` & `dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/metamaskPages/ImproveMetamaskPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.3/src/dcentralab_qa_infra_automation/pages/metamaskPages/NewToMetamaskPage.py` & `dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/metamaskPages/NewToMetamaskPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.3/src/dcentralab_qa_infra_automation/pages/metamaskPages/SwitchNetworkPage.py` & `dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/metamaskPages/SwitchNetworkPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.3/src/dcentralab_qa_infra_automation/pages/metamaskPages/WalletConnectedHomePage.py` & `dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/metamaskPages/WalletConnectedHomePage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.3/src/dcentralab_qa_infra_automation/pages/metamaskPages/WelcomeToMetamaskPage.py` & `dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/metamaskPages/WelcomeToMetamaskPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.3/src/dcentralab_qa_infra_automation/utils/HTTPMethods.py` & `dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/utils/HTTPMethods.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.3/src/dcentralab_qa_infra_automation/walletsActions/CoinbaseActions.py` & `dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/walletsActions/CoinbaseActions.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,20 @@
 from dcentralab_qa_infra_automation.pages.coinbasePages.CreatePasswordPage import CreatePasswordPage
 from dcentralab_qa_infra_automation.pages.coinbasePages.CreateWalletPage import CreateWalletPage
 from dcentralab_qa_infra_automation.pages.coinbasePages.ImportWalletPage import ImportWalletPage
 from dcentralab_qa_infra_automation.pages.coinbasePages.ReceiveCryptoToUsername import ReceiveCryptoToUsernamePage
 from dcentralab_qa_infra_automation.pages.coinbasePages.UseAnExistingWalletPage import UseAnExistingWalletPage
 from dcentralab_qa_infra_automation.pages.coinbasePages.ConfirmPage import ConfirmPage
 
+"""
+Coinbase wallet actions
+@Author: Efrat Cohen
+@Date: 03.2023
+"""
+
 
 class CoinbaseActions(WalletsActionsInterface):
     """
     coinbase actions class
     this class implements wallet actions interface.
     """
```

### Comparing `dcentralab_qa_infra_automation-1.0.3/src/dcentralab_qa_infra_automation/walletsActions/MetamaskActions.py` & `dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/walletsActions/MetamaskActions.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,20 @@
 from dcentralab_qa_infra_automation.pages.metamaskPages.ConnectWithWalletPage import ConnectWithMetamaskPage
 from dcentralab_qa_infra_automation.pages.metamaskPages.ImproveMetamaskPage import ImproveMetamaskPage
 from dcentralab_qa_infra_automation.pages.metamaskPages.NewToMetamaskPage import NewToMetamaskPage
 from dcentralab_qa_infra_automation.pages.metamaskPages.SwitchNetworkPage import SwitchNetworkPage
 from dcentralab_qa_infra_automation.pages.metamaskPages.WalletConnectedHomePage import WalletConnectedHomePage
 from dcentralab_qa_infra_automation.pages.metamaskPages.WelcomeToMetamaskPage import WelcomeToMetamaskPage
 
+"""
+MetaMask wallet actions
+@Author: Efrat Cohen
+@Date: 12.2022
+"""
+
 
 class MetamaskActions(WalletsActionsInterface):
 
     def __init__(self, driver):
         self.driver = driver
 
     def import_wallet(self):
```

### Comparing `dcentralab_qa_infra_automation-1.0.3/LICENSE` & `dcentralab_qa_infra_automation-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.3/pyproject.toml` & `dcentralab_qa_infra_automation-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "dcentralab_qa_infra_automation"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
   { name="Efrat Cohen", email="efrat.cohen@verisoft.co" },
 ]
 description = "Selenium Python Framework developed by veriSoft"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `dcentralab_qa_infra_automation-1.0.3/PKG-INFO` & `dcentralab_qa_infra_automation-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcentralab_qa_infra_automation
-Version: 1.0.3
+Version: 1.0.4
 Summary: Selenium Python Framework developed by veriSoft
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: Efrat Cohen <efrat.cohen@verisoft.co>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

