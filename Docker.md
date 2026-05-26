# Installationsguide til Docker

Følg denne guide for at installere Docker

---

## 1. Opdatér pakkelisten

```bash
sudo apt update
```

---

## 2. Installér nødvendige pakker

```bash
sudo apt install ca-certificates curl
```

---

## 3. Opret Docker keyring-mappe

```bash
sudo install -m 0755 -d /etc/apt/keyrings
```

---

## 4. Download Docker GPG-nøgle

```bash
sudo curl -fsSL https://download.docker.com/linux/ubuntu/gpg -o /etc/apt/keyrings/docker.asc
```

---

## 5. Giv læsetilladelser til nøglen

```bash
sudo chmod a+r /etc/apt/keyrings/docker.asc
```

---

## Ekstra til Docker

## Installér Docker Engine

```bash
sudo apt install docker-ce docker-ce-cli containerd.io
```

---

## Tjek Docker-version

```bash
docker --version
```

---

## Start Docker-service

```bash
sudo systemctl start docker
```

---

## Aktivér Docker ved opstart

```bash
sudo systemctl enable docker
```

---

## Vis aktive containere

```bash
docker ps
```

---

## Vis alle containere

```bash
docker ps -a
```

---

## Download et image

```bash
docker pull ubuntu
```

---

## Kør en container

```bash
docker run ubuntu
```

---

## Kør en container i baggrunden

```bash
docker run -d nginx
```

---

## Stop en container

```bash
docker stop <container-id>
```

---

## Slet en container

```bash
docker rm <container-id>
```

---

## Vis installerede images

```bash
docker images
```

---

## Slet et image

```bash
docker rmi <image-id>
```
