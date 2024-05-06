## 4. Projeto da Solução

![Uploading Dark Blue Modern Geometric Simple Feature Section Website UI Prototype.png…]()


## 4.1. Arquitetura da solução


......  COLOQUE AQUI O SEU TEXTO E O DIAGRAMA DE ARQUITETURA .......

 Inclua um diagrama da solução e descreva os módulos e as tecnologias
 que fazem parte da solução. Discorra sobre o diagrama.
 
 **Exemplo do diagrama de Arquitetura**:
 
 ![Exemplo de Arquitetura](./images/arquitetura-exemplo.png)
 

### 4.2. Protótipos de telas

 Protótipo da tela HOME:

 ![2](https://github.com/ICEI-PUC-Minas-PSG-ADS-TI/psg-ads-2024-1-p2-tiapn-7358-1-01-Afiados-Estilosos/assets/129122228/0051c434-f476-4c98-bc40-de97cc41c3bd)

 Protótipo da tela de SERVIÇOS:

 ![1](https://github.com/ICEI-PUC-Minas-PSG-ADS-TI/psg-ads-2024-1-p2-tiapn-7358-1-01-Afiados-Estilosos/assets/129122228/bbdbdc6c-8223-42bd-ba6a-4f8e9dab09cd)

Protótipo da tela de login/cadastro:

![Prototipo cadastro e login](https://github.com/ICEI-PUC-Minas-PSG-ADS-TI/psg-ads-2024-1-p2-tiapn-7358-1-01-Afiados-Estilosos/assets/129122228/d8932b39-80de-483a-b26c-de25e91b10e4)


### 4.3. Modelo de dados


![Modelo DER tiaw2](https://github.com/ICEI-PUC-Minas-PSG-ADS-TI/psg-ads-2024-1-p2-tiapn-7358-1-01-Afiados-Estilosos/assets/129122228/edf35552-3f42-4869-a1d6-702c574dc10d)



-- Table `mydb`.`agendamento`
-- -----------------------------------------------------
CREATE TABLE IF NOT EXISTS `mydb`.`agendamento` (
  `idagenda` INT NOT NULL,
  `nome` VARCHAR(45) NOT NULL,
  `servico` VARCHAR(45) NOT NULL,
  `data` DATE NOT NULL,
  `horario` VARCHAR(4) NOT NULL,
  PRIMARY KEY (`idagenda`))
ENGINE = InnoDB;


-- -----------------------------------------------------
-- Table `mydb`.`usuarios`
-- -----------------------------------------------------
CREATE TABLE IF NOT EXISTS `mydb`.`usuarios` (
  `id` INT NOT NULL,
  `nome` VARCHAR(50) NOT NULL,
  `email` VARCHAR(45) NOT NULL,
  `senha` VARCHAR(20) NOT NULL,
  `agendamento_idagenda` INT NOT NULL,
  PRIMARY KEY (`id`, `agendamento_idagenda`),
  INDEX `fk_usuarios_agendamento_idx` (`agendamento_idagenda` ASC) VISIBLE,
  CONSTRAINT `fk_usuarios_agendamento`
    FOREIGN KEY (`agendamento_idagenda`)
    REFERENCES `mydb`.`agendamento` (`idagenda`)
    ON DELETE NO ACTION
    ON UPDATE NO ACTION)
ENGINE = InnoDB;


-- -----------------------------------------------------
-- Table `mydb`.`anuncios`
-- -----------------------------------------------------
CREATE TABLE IF NOT EXISTS `mydb`.`anuncios` (
  `idanuncios` INT NOT NULL,
  `nome` VARCHAR(50) NULL,
  `foto` VARCHAR(50) NULL,
  `descricao` LONGTEXT NULL,
  PRIMARY KEY (`idanuncios`))
ENGINE = InnoDB;


-- -----------------------------------------------------
-- Table `mydb`.`servicosprecos`
-- -----------------------------------------------------
CREATE TABLE IF NOT EXISTS `mydb`.`servicosprecos` (
  `idservicos` INT NOT NULL,
  `cabelo` INT NOT NULL,
  `barba` INT NOT NULL,
  `cabelomaisbarba` INT NOT NULL,
  `sombracelha` INT NOT NULL,
  `pezinho` INT NOT NULL,
  `limpezapele` INT NOT NULL,
  `agendamento_idagenda` INT NOT NULL,
  `anuncios_idanuncios` INT NOT NULL,
  PRIMARY KEY (`idservicos`, `agendamento_idagenda`),
  INDEX `fk_servicosprecos_agendamento1_idx` (`agendamento_idagenda` ASC) VISIBLE,
  INDEX `fk_servicosprecos_anuncios1_idx` (`anuncios_idanuncios` ASC) VISIBLE,
  CONSTRAINT `fk_servicosprecos_agendamento1`
    FOREIGN KEY (`agendamento_idagenda`)
    REFERENCES `mydb`.`agendamento` (`idagenda`)
    ON DELETE NO ACTION
    ON UPDATE NO ACTION,
  CONSTRAINT `fk_servicosprecos_anuncios1`
    FOREIGN KEY (`anuncios_idanuncios`)
    REFERENCES `mydb`.`anuncios` (`idanuncios`)
    ON DELETE NO ACTION
    ON UPDATE NO ACTION)
ENGINE = InnoDB;


#### 4.3.3 Modelo Físico

C:\Users\kayla\3D Objects\BD - Diagramas de Relacionamentos



### 4.4. Tecnologias

_Descreva qual(is) tecnologias você vai usar para resolver o seu problema, ou seja, implementar a sua solução. Liste todas as tecnologias envolvidas, linguagens a serem utilizadas, serviços web, frameworks, bibliotecas, IDEs de desenvolvimento, e ferramentas._

Apresente também uma figura explicando como as tecnologias estão relacionadas ou como uma interação do usuário com o sistema vai ser conduzida, por onde ela passa até retornar uma resposta ao usuário.


| **Dimensão**   | **Tecnologia**  |
| ---            | ---             |
| SGBD           | MySQL           |
| Front end      | HTML+CSS+JS     |
| Back end       | Java SpringBoot |
| Deploy         | Github Pages    |

