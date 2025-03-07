# Selenium-ETL

# 🖥️ Selenium - Automatización Web

## 🚀 Introducción
Selenium es una biblioteca de Python que permite automatizar la interacción con navegadores web. Es útil para pruebas automatizadas, scraping de datos y tareas repetitivas en páginas web.

## 📦 Instalación
Para usar Selenium, primero hay que instalarlo con:

```sh
pip install selenium
```

También se necesita un **WebDriver** para controlar el navegador. Algunos ejemplos:
- **Chrome:** [Descargar ChromeDriver](https://sites.google.com/chromium.org/driver/)
- **Firefox:** [Descargar GeckoDriver](https://github.com/mozilla/geckodriver/releases)

Ubica el WebDriver en una carpeta accesible y usa su ruta en tu código.

## 📜 Ejemplo básico
Este código abre Google en Chrome:

```python
from selenium import webdriver

# Ruta del ChromeDriver (ajustar según tu sistema)
driver = webdriver.Chrome()

# Abrir Google
driver.get("https://www.google.com")

# Cerrar el navegador
driver.quit()
```

## 🔍 Métodos esenciales
Algunos métodos básicos en Selenium:

```python
# Encontrar elementos
boton = driver.find_element("tag name", "button")
campo = driver.find_element("name", "q")

# Interactuar con elementos
boton.click()
campo.send_keys("Hola Mundo")

# Extraer texto
titulo = driver.title
print("Título de la página:", titulo)

# Capturar pantallas
driver.save_screenshot("captura.png")
```

## 🎯 Próximos pasos
- Interacción con formularios y botones.
- Esperas dinámicas con `WebDriverWait`.
- Scraping de datos de páginas web.

---
📌 **Este repositorio busca explicar Selenium con ejemplos simples para aprender de manera práctica.**

