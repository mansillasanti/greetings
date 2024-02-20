# Saludos en Go

Este paquete proporciona una forma simple de obtener saludos personalizados en Go.

## Instalacion
Ejecuta el siguiente comando para instalar el paquete:
```bash
go get -u github.com/mansillasantiago/greetings
```

## Uso
Aqui tienes un ejemplo de como utilizar el paquete en tu codigo:

```go
package main

import(
    "fmt"
    "github.com/mansillasantiago/greetings"
)

func main(){
    message, err := greetings.Hello("Santiago")

    if err != nil {
        fmt.Println("Ocurrio un erro:", err)
        return
    }

    fmt.Println(message)
}

```
Este ejemplo importa el paquete github.com/mansillasantiago/greetings y llama a la funcion Hello() que genera un saludo personalizado. Si ocurre un erro, se imprime un mensaje de error.