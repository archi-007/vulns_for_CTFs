# Steganography

Hide code inside images and audio files, and later extract them using steghide.

## Procedure

- Install
```
apt-get install steghide
```
- Embed code
```
steghide embed -ef secret.txt -cf StegoCat.jpg -e none -Z
```
- Extract code
```
steghide extract -sf StegoCat.jpg -xf outputFile.jpg