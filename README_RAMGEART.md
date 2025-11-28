# Oh My Bash Enhanced 🚀

[![GitHub release](https://img.shields.io/github/release/ramgeart/oh-my-bash-enhanced.svg)](https://github.com/ramgeart/oh-my-bash-enhanced/releases)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## 📋 Descripción

**Oh My Bash Enhanced** es un fork mejorado del popular framework [Oh My Bash](https://github.com/ohmybash/oh-my-bash) que incluye la implementación completa de todas las funciones CLI que estaban pendientes.

## ✨ Mejoras Implementadas

Todas las funciones del comando `omb` ahora están **completamente funcionales**:

| Función | Estado | Descripción |
|---------|--------|-------------|
| `omb help` | ✅ | Ayuda completa con ejemplos |
| `omb version` | ✅ | Muestra versiones de OMB y Bash |
| `omb changelog` | ✅ | Historial de commits desde git |
| `omb plugin` | ✅ | Gestión completa de plugins |
| `omb theme` | ✅ | Gestión completa de temas |
| `omb update` | ✅ | Actualización desde repositorio git |
| `omb pull` | ✅ | Pull de cambios del repositorio |
| `omb reload` | ✅ | Recarga de configuración |

## 🚀 Instalación

### Opción 1: Instalación desde cero

```bash
bash -c "$(curl -fsSL https://raw.githubusercontent.com/ramgeart/oh-my-bash-enhanced/master/tools/install.sh)"
```

### Opción 2: Migrar desde Oh My Bash original

Si ya tienes Oh My Bash instalado:

```bash
# Haz backup de tu configuración actual
cp ~/.bashrc ~/.bashrc.backup

# Cambia al directorio de Oh My Bash
cd ~/.oh-my-bash

# Cambia el remoto al repositorio enhanced
git remote set-url origin https://github.com/ramgeart/oh-my-bash-enhanced.git

# Actualiza
git pull origin master

# Recarga tu configuración
omb reload
```

## 🔧 Uso de las Funciones CLI

### Gestión de Plugins

```bash
# Listar todos los plugins disponibles
omb plugin list

# Habilitar plugins
omb plugin enable git battery docker

# Deshabilitar plugins
omb plugin disable battery

# Obtener información de un plugin
omb plugin info git

# Cargar plugins temporalmente
omb plugin load git
```

### Gestión de Temas

```bash
# Listar temas disponibles
omb theme list

# Usar un tema temporalmente
omb theme use powerline-main

# Establecer tema permanentemente
omb theme set agnoster
```

### Actualizaciones

```bash
# Actualizar Oh My Bash Enhanced
omb update

# Solo hacer pull de cambios
omb pull

# Recargar configuración después de cambios
omb reload
```

### Información

```bash
# Ver ayuda completa
omb help

# Ver versiones
omb version

# Ver changelog
omb changelog
omb changelog master
```

## 🎨 Temas Disponibles

Oh My Bash Enhanced incluye todos los temas del original:

- **powerline-main** - Tema powerline clásico
- **agnoster** - Tema minimalista con información de git
- **font** - Tema limpio y simple
- **brainy** - Tema con múltiples segmentos configurables
- **minimal** - Tema ultra-minimalista
- Y muchos más... (85+ temas disponibles)

## 🔌 Plugins Disponibles

Plugins populares incluidos:

- **git** - Mejoras para trabajo con Git
- **battery** - Indicador de batería
- **docker** - Completado para Docker
- **python** - Soporte para entornos Python
- **npm** - Completado para NPM
- **sudo** - Alias útiles para sudo
- Y muchos más... (150+ plugins disponibles)

## 📁 Estructura del Proyecto

```
oh-my-bash/
├── lib/
│   ├── cli.bash          # 🆕 Funciones CLI implementadas
│   └── ...
├── plugins/              # 150+ plugins
├── themes/               # 85+ temas
├── completions/          # Completados para comandos
├── custom/               # Personalizaciones del usuario
├── tools/                # Herramientas y utilidades
└── oh-my-bash.sh         # Script principal
```

## 🛠️ Características Técnicas

- ✅ **Manejo de errores robusto** - Todas las funciones incluyen verificación de errores
- ✅ **Soporte para customizaciones** - Funciona con archivos en `OSH_CUSTOM`
- ✅ **Mensajes descriptivos** - Feedback claro sobre operaciones realizadas
- ✅ **Compatibilidad** - Totalmente compatible con la configuración existente
- ✅ **Git integration** - Aprovecha el repositorio git para actualizaciones

## 🤝 Contribuir

¡Las contribuciones son bienvenidas! Por favor:

1. Fork el repositorio
2. Crea una rama para tu feature (`git checkout -b feature/amazing-feature`)
3. Commit tus cambios (`git commit -m 'Add some amazing feature'`)
4. Push a la rama (`git push origin feature/amazing-feature`)
5. Abre un Pull Request

## 📄 Licencia

Este proyecto mantiene la licencia MIT del proyecto original.

## 🙏 Agradecimientos

- [Oh My Bash Original](https://github.com/ohmybash/oh-my-bash) - El framework que hizo posible esto
- [Oh My Zsh](https://github.com/ohmyzsh/ohmyzsh) - La inspiración original

## 📞 Soporte

- 📧 Reporta issues en: [GitHub Issues](https://github.com/ramgeart/oh-my-bash-enhanced/issues)
- 💬 Discusiones: [GitHub Discussions](https://github.com/ramgeart/oh-my-bash-enhanced/discussions)

---

**⭐ Si este proyecto te es útil, no olvides darle una estrella!**