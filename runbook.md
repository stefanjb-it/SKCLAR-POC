# Presentation runbook:

- Repo fork: https://github.com/stefanjb-it/SKCLAR-POC
- az login
- az account list
- az account --set-subscription c42c6aa8-3c10-40e5-a3ff-ba5843e3dda5
- az ad sp create-for-rbac --name "SKCLAR-POC" --role contributor --scopes /subscriptions/c42c6aa8-3c10-40e5-a3ff-ba5843e3dda5/resourceGroups/CLINF_GL-[NAME] --sdk-auth
- Github secret hinzufügen:
  - name: AZURE_CREDENTIALS_AZURECLI
  - value: CLI Ergebnis
- Actions öffnen und bestätigen
- deploy_manual_azurecli
  - Parameter: 1 - 3 VMs (weniger ist besser)
- Azure portal öffnen: https://portal.azure.com
- RG öffnen und warten bis Actions fertig ist
- Aktualisieren, Frontend IP aus Loadbalancer kopieren und Webseite öffnen
- Zurück zu Github Actions
- clear_manual_azurecli starten und laufen lassen
- Wenn Action fertig ist Resourcegroup überprüfen ob alles gelöscht wurde
