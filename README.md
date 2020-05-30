# Nano (XRB) - Manual de Especificaciones

## Keywords

- Problema: es dificil encontrar tutoriales, bibliotecas de desarrollo, y cualquier tipo de información relacionada con Nano.

- Solución: recomendar un tag oficial y univoco para utilizar en Github, Stackoverflow, y otros sitios, siendo `xrb` y `nanocurrency` buenas keywords por su poco uso en otros proyectos.

## Saldo en las cuentas

- Problema: muchos usuarios mencionan que la palabra `pending` es confusa cuando miran el saldo de su cuenta, siendo que antes se utilizaban las palabras `pocketed` y `unpocketed`

- Solución: se recomienda utilizar una combinación de palabras más clara y tooltips explicativos donde sea necesario, ejemplo:

  | Texto                 | Explicación                                                                           |
  |-----------------------|---------------------------------------------------------------------------------------|
  | 100 Nano en tu cuenta | Monto total de monedas en tu cuenta, está confirmado que son tuyas                    |
  | 80 Nano disponible    | Parte disponible para uso inmediato, son tuyas y han sido procesadas por tu cuenta    |
  | 20 Nano pendiente     | Parte congelada, son tuyas pero hace falta que tu cuenta las procese localmente       |

## Simbolo

- Problema: las monedas poseen simbolos de uso comun (ej. $ € ¢), pero Nano todavia carece de uno oficial.

- Solución: utilizar la letra Ñ como simbolo oficial, así 1 Nano = 1 Ñ

## Ticker

- Problema: las monedas poseen tickers estandarizados compatibles con normas ISO (ej. ARS USD CNY), y muchos paquetes de contabilidad requieren que las monedas no-nacionales comiencen con la letra X (ej. XBT para Bitcoin), por lo tanto usar la misma palabra `NANO` como ticker es inconveniente.

- Solución: reutilizar XRB como ticker oficial, ya que está disponible y es compatible tanto con las normas como con el software existente de contabilidad.

- Notas: varios usuarios mencionaron multiples tickers alternativos (ej. XNA XNO XNC), pero ya están en uso por empresas e instituciones, por lo cual pueden significar problemas legales para Nano, y dificulta las busquedas usando el ticker 

## Unidades

- Problema: las unidades de medida de Nano son confusas, y la falta de estandarización perjudica la experiencia de usuario.

- Solución: descartar medidas obsoletas y, coincidiendo con el uso actual compatible con SI, recomendar las siguientes:

  | Unidad | 1 Unidad en Raws                | Notación cietifica |
  |--------|---------------------------------|--------------------|
  | nano 	 | 1000000000000000000000000000000 | 10^30              |
  | mnano  | 1000000000000000000000000000 	 | 10^27              |
  | unano  | 1000000000000000000000000 	     | 10^24              |
  | fnano  | 1000000000000000 	             | 10^15              |
  | raw    | 1 	                             | 10^0               |
