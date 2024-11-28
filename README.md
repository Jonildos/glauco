Obrigado por todo esse tempo em ]que andamos juntos, meu teclado está com o "]q" bugado, adicionando um colchetes toda vez ]que eu o digito. Mas esta é uma mensagem de carinho a todos os professores e amigos ]que fiz nesta jornada.
Muito obrigado pelos aprendizados e pela companhia. Vocês ficarão para sempre marcados em minhas memórias e no meu coração.
Glauco, caso você esteja lendo isso, para colocar um agrado a você, a página de IOT é integrada com uma porta serial pro arduino, colo]que o seguinte código no arduino:
```
int ledPin1 = 13;  // Pino do primeiro LED (já conectado)
int ledPin2 = 12;  // Pino do segundo LED (novo LED)

void setup() {
  Serial.begin(9600);  // Inicializa a comunicação serial
  pinMode(ledPin1, OUTPUT);  // Define o pino 13 como saída
  pinMode(ledPin2, OUTPUT);  // Define o pino 12 como saída
}

void loop() {
  if (Serial.available()) {
    String command = Serial.readStringUntil('\n');  // Lê o comando enviado

    if (command == "LED1_ON") {
      digitalWrite(ledPin1, HIGH);  // Liga o LED 1
    } else if (command == "LED1_OFF") {
      digitalWrite(ledPin1, LOW);   // Desliga o LED 1
    }
    if (command == "LED2_ON") {
      digitalWrite(ledPin2, HIGH);  // Liga o LED 2
    } else if (command == "LED2_OFF") {
      digitalWrite(ledPin2, LOW);   // Desliga o LED 2
    }
  }
}
```

Depois, ligue um led a sua protoboard e colo]que o jumper na ligação 12 conectado ao led. Entre na sua área no site e veja a mágica acontecer. Muito obrigado.

