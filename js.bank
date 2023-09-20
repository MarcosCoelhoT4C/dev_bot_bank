
const readline = require('readline');
const rl = readline.createInterface({
  
  input

 
input: process.stdin,
  
  output
output: process.stdout
});

function getUserName() {
  rl.
  rl

question('Por favor, digite seu nome: ', (name) => {
    
console.log(`Olá, ${name}!`);
    
    checkBusinessHours

    checkBusiness

   
//v1.2
// The default offset if the offset has not been set
const DEFAULT_OFFSET = -3;

// Receive the variables as parameters
function run(offset, weekSchedule) {
   
    offset = !isNaN(parseInt(offset))? parseInt(offset) : DEFAULT_OFFSET;
    
    weekSchedule = JSON.parse(weekSchedule);
    let today = nowUTC(offset);
    if (isWorkDay(today, weekSchedule)) {
        let todaySchedule = getTodaySchedule(weekSchedule, today);
        let intervalTime = getIntervalTime(todaySchedule, today);
        return checkTime(intervalTime, today);
    }
    return false;
}
function getIntervalTime(todaySchedule, today) {
    let intervalTime = [];
    for (let i = 0; i < todaySchedule.workTime.length; i++) {
        intervalTime.push({
            start: utcDate(todaySchedule.workTime[i].start, today),
            end: utcDate(todaySchedule.workTime[i].end, today)
        });
    }
    return intervalTime;
}
function checkTime(intervalTime, today) {
    for (let i = 0; i < intervalTime.length; i++) {
        if (today - intervalTime[i].start > 0 && intervalTime[i].end - today > 0)
            return true;
    }
    return false;
}
function getTodaySchedule(weekSchedule, today) {
    for (let i = 0; i < weekSchedule.length; i++) {
        if (weekSchedule[i].num == today.getDay()) return weekSchedule[i];
    }
}
//Get now UTC Date
function nowUTC(offset) {
    let now = new Date();
    let utc_timestamp = Date.UTC(
        now.getUTCFullYear(),
        now.getUTCMonth(),
        now.getUTCDate(),
        now.getUTCHours(),
        now.getUTCMinutes(),
        now.getUTCSeconds(),
        now.getUTCMilliseconds()
    );
    return new Date(utc_timestamp + offset * 3600 * 1000);
}
//Get UTC Date
function utcDate(timeString, today) {
    let hour = getValueByString("hour", timeString);
    let minutes = getValueByString("minutes", timeString);
    let utc_timestamp = Date.UTC(
        today.getUTCFullYear(),
        today.getUTCMonth(),
        today.getUTCDate(),
        hour,
        minutes,
        0,
        0
    );
    return new Date(utc_timestamp);
}
//Get hour/minute by string with pattern HH:mm
function getValueByString(type, timeString) {
    if (type === "hour") {
        return parseInt(timeString.substring(0, timeString.indexOf(":")));
    } else if (type === "minutes") {
        return parseInt(
            timeString.substring(timeString.indexOf(":") + 1, timeString.length)
        );
    }
    return 0;
}
//Get if today is a work day
function isWorkDay(today, workDays) {
    for (let i = 0; i < workDays.length; i++) {
        if (workDays[i].num == today.getDay().toString()) return true;
    }
    return false;
}

function run() {
 let workSchedule = [
    {
        "num": 1,
        "name": "Monday",
        "portugueseName": "Segunda",
        "workTime": [
            {
                "start": "08:00",
                "end": "18:00"
            }
        ]
    },
    {
        "num": 2,
        "name": "Tuesday",
        "portugueseName": "Terça",
        "workTime": [
            {
                "start": "08:00",
                "end": "18:00"
            }
        ]
    },
    {
        "num": 3,
        "name": "Wednesday",
        "portugueseName": "Quarta",
        "workTime": [
            {
                "start": "08:00",
                "end": "18:00"
            }
        ]
    },
    {
        "num": 4,
        "name": "Thursday",
        "portugueseName": "Quinta",
        "workTime": [
            {
                "start": "08:00",
                "end": "18:00"
            }
        ]
    },
    {
        "num": 5,
        "name": "Friday",
        "portugueseName": "Sexta",
        "workTime": [
            {
                "start": "08:00",
                "end": "18:00"
            }
        ]
    },
  
 return JSON.stringify(workSchedule); //Return value will be saved as "Return value variable" field name
 }
    showMainMenu

   
showMainMenu();
  } 
  }
else {
    console.log('Desculpe, se você precisa falar com um dos nossos especialistas o horário de atendimento é das 9h às 18h.');
    rl.
    rl

   
close();
  }
}

// Função para mostrar o menu de opções
function showMainMenu() {
  console.log('Menu de Opções:');
  console.log('1. Saldo');
  
 
console.log('2. Extrato');
  console.log('3. Solicitar 2ª Via de Cartão');
  console.log('4. Solicitar Empréstimo Consignado');
  
 
console.log('5. Sair');

  rl.

  rl

question('Por favor, escolha uma opção (1-5): ', (choice) => {
    switch (choice) {
      
     
case '1':
        
       
// Lógica para verificar saldo
        rl.
       
question('Digite o número da sua conta: ', (accountNumber) => {
          rl.
         
question('Digite seu login: ', (login) => {
            
            check
checkBalance(accountNumber, login);
          });
        });
        
          });
        });
       

          });
        });

          });
       

          });

         
break;
      case '2':
        rl.question('Digite o número da sua conta: ', (accountNumber) => {
          rl.
          rl

         
question('Digite seu login: ', (login) => {
            showStatement(accountNumber, login);
          });
        });
        
          });
        });
break;
      case '3':
        rl.
       
question('Digite o número da sua conta: ', (accountNumber) => {
          rl.
         
question('Digite seu login: ', (login) => {
            
           
requestCardReplacement(accountNumber, login);
          });
        });
        
          });
        });
       
break;
      
     
case '4':
        rl.
        rl

       
question('Digite o número da sua conta: ', (accountNumber) => {
          rl.
          rl

         
question('Digite seu login: ', (login) => {
            requestLoan(accountNumber, login);
          });
        });
        break;
      case '5':
        console.log('Obrigado por usar nossos serviços. Até mais!');
        rl.
       
close();
        break;
      default:
        
       
console.log('Opção inválida. Por favor, escolha uma opção válida.');
        showMainMenu();
    }
  });
}


    }
// Lógica para verificar saldo
function checkBalance(accountNumber, login) {  
 
const saldo = 1000; 
  console.log(`Seu saldo atual é de R$ ${saldo}`);
  showMainMenu();
}

function showStatement(accountNumber, login) {
  
  const extrato = [
    { data: '2023-09-20', descricao: 'Compra em loja X', valor: -50 },
    { data: '2023-09-19', descricao: 'Depósito', valor: 1000 },
    
   
// ... Outras transações
  ];

  console.log('Extrato da conta:');
  extrato.
  extr
forEach((transacao) => {
    console.log(`Data: ${transacao.data}, Descrição: ${transacao.descricao}, Valor: R$ ${transacao.valor}`);
  });

  showMainMenu();
}

function requestCardReplacement(accountNumber, login) {

  console.log('Sua solicitação para a 2ª via do cartão foi recebida. Em breve, entraremos em contato para mais detalhes.');
  showMainMenu();
}

function requestLoan(accountNumber, login) {
  console.log('Sua solicitação de empréstimo consignado foi recebida. Aguarde a análise e aprovação.');
  
  show
showMainMenu();
}

// Iniciar o processo
getUserName();
