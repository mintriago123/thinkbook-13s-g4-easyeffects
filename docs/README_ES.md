# Perfiles de EasyEffects para Lenovo ThinkBook 13s G4 ARB

[![Licencia: MIT](https://img.shields.io/badge/Licencia-MIT-yellow.svg)](../LICENSE)
[![GitHub stars](https://img.shields.io/github/stars/mintriago123/thinkbook-13s-g4-easyeffects?style=social)](https://github.com/mintriago123/thinkbook-13s-g4-easyeffects)
[![Versión Realtek](https://img.shields.io/badge/Realtek-6.0.9430.1-blue)](https://download.lenovo.com/consumer/mobiles/g0t1077fmyebg9d0.exe)

[English version](../README.md) | Versión en Español

Perfiles de audio optimizados para EasyEffects basados en el driver de audio Realtek oficial de la Lenovo ThinkBook 13s G4 ARB.

> ⚠️ **DESCARGO DE RESPONSABILIDAD**: Estos perfiles se proporcionan "tal cual" sin garantía de ningún tipo. Úsalos bajo tu propio riesgo. El autor no es responsable de ningún daño a tu hardware, software o audición. Siempre usa niveles de volumen razonables y prueba los perfiles a volumen bajo primero.

## 📋 Descripción

Este repositorio contiene perfiles de audio extraídos del driver oficial de Realtek para la ThinkBook 13s G4 ARB, convertidos para su uso con EasyEffects en Linux. Los perfiles están optimizados para diferentes escenarios de uso y replican la experiencia de audio del driver oficial de Windows.

## 🎵 Perfiles Disponibles

| Perfil | Archivo | Mejor Para | Bajos | Agudos | Claridad |
|--------|---------|------------|-------|--------|----------|
| **Game** | `Thinkbook13s_Arb_Game.json` | Juegos, FPS | 🔊🔊🔊 | 🔊🔊🔊 | ⭐⭐⭐ |
| **Movie** | `Thinkbook13s_Arb_Movie.json` | Películas, Series | 🔊🔊🔊🔊 | 🔊🔊 | ⭐⭐⭐⭐ |
| **Music** | `Thinkbook13s_Arb_Music.json` | Escuchar música | 🔊🔊🔊 | 🔊🔊🔊🔊 | ⭐⭐⭐⭐⭐ |
| **Universal** | `Thinkbook13s_Arb_Universal.json` | Uso diario | 🔊🔊 | 🔊🔊 | ⭐⭐⭐ |
| **Voice** | `Thinkbook13s_Arb_Voice.json` | Videollamadas | 🔊 | 🔊🔊 | ⭐⭐⭐⭐⭐ |

## 💻 Compatibilidad

### Hardware
- **Modelo**: Lenovo ThinkBook 13s G4 ARB
- **Chipset de Audio**: Realtek (PCI Subsystem ID: 17AA:3844)

### Software
- **Sistema Operativo**: Linux (cualquier distribución)
- **Requisito**: EasyEffects instalado
- **Basado en**: Realtek Audio Driver 6.0.9430.1 para Windows 11 (64-bit)

## 📦 Instalación

### Prerrequisitos

1. Instalar EasyEffects en tu sistema:

```bash
# Ubuntu/Debian
sudo add-apt-repository ppa:apandada1/easyeffects
sudo apt update
sudo apt install easyeffects lsp-plugins-lv2 calf-plugins zam-plugins rubberband-cli libzita-convolver-dev librnnoise-dev

# Fedora
sudo dnf install easyeffects lsp-plugins-lv2 calf zam-plugins lv2-mdala-plugins rubberband zita-convolver rnnoise

# Arch Linux
sudo pacman -S easyeffects lsp-plugins-lv2 calf zam-plugins-lv2 rubberband zita-convolver rnnoise
yay -S lv2-mdala-plugins

# Flatpak (cualquier distribución)
flatpak install flathub com.github.wwmm.easyeffects
```

### Instalación de Perfiles

1. Clona este repositorio:
```bash
git clone https://github.com/mintriago123/thinkbook-13s-g4-easyeffects.git
cd thinkbook-13s-g4-easyeffects
```

2. Copia los perfiles a la carpeta de configuración de EasyEffects:

   **Instalación nativa:**
   ```bash
   mkdir -p ~/.config/easyeffects/output
   cp profiles/*.json ~/.config/easyeffects/output/
   ```

   **Instalación Flatpak:**
   ```bash
   mkdir -p ~/.var/app/com.github.wwmm.easyeffects/config/easyeffects/output
   cp profiles/*.json ~/.var/app/com.github.wwmm.easyeffects/config/easyeffects/output/
   ```

3. Abre EasyEffects y selecciona el perfil deseado desde la interfaz.

## 🔧 Uso

1. Inicia EasyEffects
2. En el menú de perfiles, selecciona el perfil según tu actividad:
   - **Game**: Para sesiones de juego con audio inmersivo
   - **Movie**: Para disfrutar películas con audio envolvente
   - **Music**: Para una experiencia de audio Hi-Fi al escuchar música
   - **Universal**: Para uso diario y multitarea
   - **Voice**: Para videollamadas con claridad vocal optimizada

## 📄 Archivo de Configuración Original

El archivo [`drivers/DEV_0287_SUBSYS_17AA3844_PCI_SUBSYS_382717AA.xml`](../drivers/DEV_0287_SUBSYS_17AA3844_PCI_SUBSYS_382717AA.xml) contiene la configuración original extraída del driver de Realtek que se utilizó como base para crear estos perfiles.

## 📚 Información del Driver Original

- **Versión del Driver**: Realtek 6.0.9430.1
- **Fecha de Lanzamiento**: 25 de julio de 2025
- **Tamaño**: 146.01 MB
- **Sistema Operativo**: Windows 11 (64-bit)
- **Tipo**: Recomendado

### Enlaces Oficiales

- **Descarga Directa**: [Driver de Audio Realtek](https://download.lenovo.com/consumer/mobiles/g0t1077fmyebg9d0.exe)
- **Página de Soporte**: [Lenovo ThinkBook 13s G4 ARB - Drivers](https://pcsupport.lenovo.com/ec/es/products/laptops-and-netbooks/thinkbook-series/thinkbook-13s-g4-arb/downloads/driver-list/component?name=audio&id=3AA7F1C4-5B2A-453C-9CE2-B8FCDA8B69BA)

## 🛠️ Personalización

Los perfiles pueden ser editados según tus preferencias:

1. Abre EasyEffects
2. Carga el perfil que deseas modificar
3. Ajusta los parámetros de los efectos a tu gusto
4. Guarda el perfil con un nuevo nombre o sobrescribe el existente

## ⚠️ Notas

- Estos perfiles fueron extraídos del driver oficial de Windows y adaptados para Linux
- El rendimiento puede variar según tu configuración de hardware y software
- Se recomienda probar diferentes perfiles para encontrar el que mejor se adapte a tus necesidades

## ❓ Preguntas Frecuentes

**P: ¿Estos perfiles funcionan en otros modelos Lenovo?**  
R: Están optimizados para ThinkBook 13s G4 ARB con Realtek ALC287, pero pueden funcionar en sistemas similares con el mismo chipset de audio.

**P: ¿Puedo usar estos con PulseEffects?**  
R: Estos están diseñados para EasyEffects (PipeWire). Para PulseAudio/PulseEffects, pueden requerir algunos ajustes.

**P: ¿Estos perfiles pueden dañar mis bocinas?**  
R: No, son perfiles seguros extraídos de drivers oficiales. Sin embargo, siempre usa niveles de volumen razonables para proteger tu audición y hardware.

**P: ¿Por qué necesito instalar EasyEffects?**  
R: EasyEffects es la herramienta de procesamiento de audio que aplica estos perfiles. Es el equivalente en Linux del software Dolby Atmos en Windows.

**P: ¿Puedo modificar estos perfiles?**  
R: ¡Por supuesto! Estos son puntos de partida. Siéntete libre de personalizarlos según tus preferencias a través de la interfaz de EasyEffects.

## 🤝 Contribuciones

Las contribuciones son bienvenidas. Si has creado un perfil personalizado o mejorado uno existente, no dudes en enviar un pull request.

## ⚖️ Licencia y Aspectos Legales

Este proyecto está licenciado bajo la **Licencia MIT** - consulta el archivo [LICENSE](../LICENSE) para más detalles.

### Descargo de Responsabilidad Legal

Estos perfiles de audio fueron extraídos de los drivers oficiales de Realtek que contienen afinación Dolby Atmos. Se proporcionan para uso educativo y personal bajo principios de uso justo para interoperabilidad en sistemas Linux.

- **Dolby Atmos** es una marca registrada de Dolby Laboratories
- **Realtek** es una marca registrada de Realtek Semiconductor Corp.
- No afiliado con Dolby, Realtek o Lenovo

Consulta [DISCLAIMER.md](../DISCLAIMER.md) para información legal completa.

## 📧 Soporte

Si encuentras problemas o tienes preguntas, por favor abre un issue en este repositorio.

---

**Nota**: Este proyecto no está afiliado oficialmente con Lenovo o Realtek. Los perfiles son recreaciones basadas en el driver oficial para mejorar la experiencia de audio en Linux.
