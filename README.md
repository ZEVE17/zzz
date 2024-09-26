Proceso DibujarFlor
    Definir radio, num_petalos, angulo_completo, angulo_petalos Como Real
    radio = 100
    num_petalos = 6
    angulo_completo = 360
    angulo_petalos = angulo_completo / num_petalos

    // Inicializar la tortuga
    TortugaIniciar()
    TortugaPosicion(0, 0) // Coloca la tortuga en el centro
    TortugaVelocidadMaxima()

    // Dibujar los pétalos
    Para i=1 Hasta num_petalos Con Paso 1 Hacer
        // Dibujar el primer arco del pétalo
        TortugaGirarIzquierda(angulo_petalos / 2) // Gira un poco para iniciar el pétalo
        Para j=1 Hasta 180 Con Paso 1 Hacer
            TortugaAvanzar(1) // Avanza 1 unidad
            TortugaGirarDerecha(1) // Gira suavemente para formar el arco
        FinPara

        // Dibujar el segundo arco del pétalo
        Para j=1 Hasta 180 Con Paso 1 Hacer
            TortugaAvanzar(1) // Avanza 1 unidad
            TortugaGirarDerecha(1) // Sigue girando suavemente
        FinPara

        // Girar para el siguiente pétalo
        TortugaGirarIzquierda(angulo_petalos)
    FinPara

    // Finalizar el dibujo
    TortugaFinalizar()
FinProceso
