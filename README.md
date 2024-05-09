# deteccao_facial
Em resumo, o código captura o vídeo da webcam, detecta os rostos em cada frame e exibe o vídeo resultante com os retângulos ao redor dos rostos. O loop é encerrado quando a tecla 'ESC' é pressionada.

Este código utiliza a biblioteca OpenCV e um módulo de detecção de rostos (FaceDetectionModule) para detectar rostos em um vídeo em tempo real a partir da webcam. Aqui está uma descrição passo a passo do que o código faz:

1. Importa as bibliotecas necessárias:
  cv2: para processamento de vídeo e imagens.
  FaceDetector do módulo cvzone.FaceDetectionModule: uma classe que simplifica a detecção de rostos.

2. Inicializa a captura de vídeo utilizando a webcam padrão (índice 0).
3. Instancia o objeto FaceDetector para detectar rostos.
4. Entra em um loop infinito:
  Lê o próximo frame do vídeo usando video.read(), armazenando-o em img.
  Chama o método detector.findFaces(img, draw=True) para detectar rostos na imagem. O parâmetro draw=True indica que os retângulos ao redor dos rostos devem ser desenhados na imagem.
  Mostra a imagem resultante com os retângulos dos rostos usando cv2.imshow().
  Aguarda a tecla pressionada com cv2.waitKey(1). Se a tecla 'ESC' (código 27) for pressionada, o loop é interrompido.
5. Quando o loop é interrompido (tecla 'ESC' pressionada), o vídeo é liberado com video.release() e todas as janelas abertas são fechadas com cv2.destroyAllWindows().

Em resumo, o código captura o vídeo da webcam, detecta os rostos em cada frame e exibe o vídeo resultante com os retângulos ao redor dos rostos. O loop é encerrado quando a tecla 'ESC' é pressionada.






