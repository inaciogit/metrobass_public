# 🎸 Metro Bass

**Curso Anual de Leitura para Contrabaixo**

Aplicativo desktop para aprender leitura de partitura no contrabaixo, do básico ao avançado, com metrônomo, editor de partitura, quiz e curso de 60 semanas.


## Sobre o projeto

O Metro Bass organiza um curso de 12 meses, dividido em 2 módulos e 5 níveis. A rotina sugerida é de aproximadamente 30 minutos por dia.

O curso usa progressão gradual, revisão espaçada, exercícios de primeira vista e consolidação antes de liberar novas semanas.

## Funcionalidades

- **Curso:** 60 semanas de conteúdo progressivo.
- **Módulo A:** fundamentos ao nível intermediário, com leitura de notas, ritmos, compassos e estilos de baixo.
- **Módulo B:** performance avançada, técnica, ghost notes, walking bass, harmonia e acid jazz.
- **Metrônomo:** 30–300 BPM, compassos, subdivisões, acentos e cronômetro.
- **Editor de partitura:** modos uniforme e misto, notas, pausas e clave de fá.
- **Quiz e teoria:** reconhecimento de notas, pauta, clave de fá, compassos e posições no braço.
- **Rotina diária:** cinco blocos, revisão espaçada e controle de progresso.
- **Repertório:** seis músicas progressivas e níveis de domínio.
- **Progresso:** salvamento em JSON com backups.
- **Modo desenvolvedor:** `python main.py --dev`.

## Requisitos

- Python 3.10 ou superior
- Windows 10+, macOS 11+ ou Linux
- Aproximadamente 50 MB de espaço em disco

Principais dependências: `customtkinter`, `numpy`, `sounddevice` e `Pillow`. O `cairosvg` é opcional.

## Instalação

### Windows — PowerShell

```powershell
git clone https://github.com/SEU-USUARIO/metro-bass.git
cd metro-bass
python -m venv .venv
.\.venv\Scripts\Activate.ps1
pip install -e .
```

Para instalar também as dependências de desenvolvimento:

```powershell
pip install -e ".[dev]"
```

> Substitua `SEU-USUARIO` pelo seu nome de usuário do GitHub e confirme o nome do repositório.

## Executar

Iniciar o aplicativo:

```powershell
python main.py
```

Iniciar em modo desenvolvedor:

```powershell
python main.py --dev
```

Validar o conteúdo pedagógico:

```powershell
python scripts/validate_content.py
```


## Navegação

O aplicativo possui sete áreas principais:

1. **Curso** — semanas e lições.
2. **Quiz** — reconhecimento de notas e teoria.
3. **Diário** — rotina de prática.
4. **Repertório** — músicas e linhas de baixo.
5. **Metrônomo** — andamento e marcação do tempo.
6. **Partitura** — editor musical.
7. **Progresso** — estatísticas de aprendizagem.

Atalhos: `Espaço` inicia/pausa o metrônomo; `Esc` o interrompe.

## Estrutura do projeto

```text
metro-bass/
├── main.py
├── pyproject.toml
├── README.md
├── CHANGELOG.md
├── src/curso_baixo/
│   ├── shared/
│   ├── domain/
│   ├── infrastructure/
│   ├── application/
│   ├── presentation/
│   └── content/
├── assets/
│   └── notation/clefs/
├── docs/
│   └── curso.md
├── scripts/
│   ├── validate_content.py
│   └── generate_bass_clef_png.py
└── tests/
```

O projeto separa apresentação, casos de uso, regras de domínio e infraestrutura. O domínio não deve depender da interface gráfica ou dos recursos de áudio.

## Desenvolvimento

Execute o validador antes de enviar alterações:

```powershell
python scripts/validate_content.py
python scripts/validate_content.py --verbose
```


## Documentação

- `docs/curso.md` — plano pedagógico.
- `CHANGELOG.md` — histórico de versões.

## Licença

# LICENÇA DE USO DE SOFTWARE — METRO BASS


**Tipo de licença:** Proprietária, comercial e de código fechado.

## 1. Propriedade intelectual

O Metro Bass é um software proprietário. Seu código-fonte, estrutura, interface, recursos, documentação e demais componentes protegidos pertencem ao titular dos direitos ou a seus respectivos licenciantes.

A aquisição de uma licença não transfere ao comprador a propriedade intelectual do software nem os direitos sobre seu código-fonte.

## 2. Concessão da licença

Após a confirmação do pagamento, o titular concede ao comprador uma licença de uso do Metro Bass, conforme as condições da modalidade adquirida.

A licença autoriza o uso do programa para fins pessoais ou profissionais, respeitadas as condições comerciais informadas no momento da compra.

## 3. Restrições de uso

É proibido ao licenciado, salvo autorização prévia e expressa do titular ou quando permitido pela legislação aplicável:

- Copiar, publicar, distribuir ou revender o software, integralmente ou em partes.
- Compartilhar, sublicenciar ou transferir a licença a terceiros.
- Modificar, adaptar ou criar versões derivadas do software.
- Tentar obter, extrair ou reconstruir o código-fonte por engenharia reversa.
- Remover avisos de propriedade intelectual ou mecanismos de licenciamento.
- Utilizar o software para violar direitos de terceiros ou a legislação aplicável.

## 4. Código-fonte e distribuição

O Metro Bass é distribuído em formato executável ou por outro meio autorizado pelo titular. A compra da licença não dá direito ao acesso ao código-fonte, salvo acordo escrito em contrário.

O titular poderá manter o código-fonte em repositório privado para desenvolvimento, manutenção e atualização do produto.

## 5. Atualizações e suporte

Atualizações, novas funcionalidades, manutenção e suporte técnico serão fornecidos conforme as condições da modalidade de licença adquirida. Não há garantia de atualizações gratuitas ou suporte contínuo, salvo quando expressamente informado na oferta ou contratado separadamente.

## 6. Prazo e validade

A validade da licença — permanente ou por período determinado — será aquela informada no momento da compra.

O titular poderá suspender ou encerrar a licença em caso de violação material destes termos, observada a legislação aplicável e os direitos do consumidor.

## 7. Garantias e responsabilidade

O software é fornecido para fins de estudo e prática musical. O titular não garante resultados específicos de aprendizagem, desempenho musical ou evolução técnica.

Na extensão permitida pela legislação aplicável, o titular não será responsável por danos indiretos decorrentes do uso ou da impossibilidade de uso do programa. Esta cláusula não exclui responsabilidades que legalmente não possam ser afastadas.

## 8. Direitos legais

Esta licença não elimina nem restringe direitos assegurados ao consumidor ou outros direitos obrigatórios previstos na legislação aplicável.

## 9. Aceitação

Ao instalar, ativar ou utilizar o Metro Bass, o licenciado declara ter tido acesso a estes termos e concordar com suas condições, sem prejuízo dos requisitos legais aplicáveis à validade desse consentimento.
