# Wymagane narzedzia

W celu wzięcia udziału w warsztacie, wymagane będzie zainstalowanie następujących narzędzi na swoim komputerze:

-   aws-cli
    -   [https://aws.amazon.com/cli/](https://aws.amazon.com/cli/)
-   kubectl
    -   [Install kubectl on Linux](https://kubernetes.io/docs/tasks/tools/install-kubectl-linux)
    -   [Install kubectl on macOS](https://kubernetes.io/docs/tasks/tools/install-kubectl-macos)
    -   [Install kubectl on Windows](https://kubernetes.io/docs/tasks/tools/install-kubectl-windows)
-   helm
    -   [https://github.com/helm/helm/releases](https://github.com/helm/helm/releases)
-   lens
    -   [https://k8slens.dev/](https://k8slens.dev/)
-   docker
    -   [Docker on Ubuntu](https://docs.docker.com/engine/install/ubuntu/)
    -   [Docker Desktop for Mac](https://docs.docker.com/desktop/install/mac-install/)
    -   [Alternatywnie dla Mac: Colima](https://github.com/abiosoft/colima)
    -   [Docker Desktop on Windows](https://docs.docker.com/desktop/install/windows-install/)

Podczas warsztatu ćwiczenia bedą wykonywane na współdzielonym klastrze Kubernetes w AWS. Nie ma potrzeby instalowania własnego lokalnego klastra.

Użytkownikom Windows może być przydatny shell kompatybilny z bashem, np. git-bash albo WSL.

## Weryfikacja działania narzędzi

### aws-cli

Polecenie `aws --version` zwróci wersję aplikacji, 2.7.x lub wyższą.

```
-> aws --version
aws-cli/2.7.27 Python/3.9.11 Linux/5.19.0-2-amd64 exe/x86_64.debian prompt/off
```

### kubectl

Polecenie `kubectl version --client --short` zwróci wersję narzędzia, v1.20.x lub wyższą.
```
-> kubectl version --client --short
Client Version: v1.20.2
```

### helm

Polecenie `helm version --short` zwróci wersję, v3.7.x lub wyższą.
```
-> helm version --short
v3.7.1+g1d11fcb
```

### docker

Polecenie `docker pull nginx:latest` skutecznie pobierze obraz dockerowy z publicznego registry.
```
-> docker pull nginx:latest
latest: Pulling from library/nginx
e9995326b091: Pull complete 
71689475aec2: Pull complete 
f88a23025338: Pull complete 
0df440342e26: Pull complete 
eef26ceb3309: Pull complete 
8e3ed6a9e43a: Pull complete 
Digest: sha256:47a8d86548c232e44625d813b45fd92e81d07c639092cd1f9a49d98e1fb5f737
Status: Downloaded newer image for nginx:latest
docker.io/library/nginx:latest
```
