pipeline {
    agent any
    
    environment {
        PATH = "C:\\Program Files\\Java\\jdk-21\\bin;${env.PATH}"
        PHP_PATH = "E:\\xampp\\php"
        COMPOSER_HOME = "C:\\Users\\Administrator\\AppData\\Roaming\\Composer"
        PROJECT_DIR = "E:\\PRAN-RFL\\practise\\CI-CD"
        JENKINS_DIR = "C:\\ProgramData\\Jenkins\\.jenkins\\workspace\\LaravelTest"
        SSH_CREDENTIALS = credentials('crm-test')
    }

    stages {
        stage("For Main") {
            steps {
                script {
                    sshagent(credentials: ['b3BlbnNzaC1rZXktdjEAAAAABG5vbmUAAAAEbm9uZQAAAAAAAAABAAACFwAAAAdzc2gtcn
NhAAAAAwEAAQAAAgEAsTo5Y2iEpAt52qMDXMmqWf7pTExNwRWqWNtwjlFzUrO2F/D8wKRM
qU1lT+GTaAt2/+Nyyt0dZ3j5UMgIXhHmAcuuHlRYzir9MuCmKZXrnq3Tu2RTftbZMbL5MV
UXqK0WR57dDqQL5oG5ILdBsT+lpAtOjoLj9Lf593JlMH4MbY6XcNbxxFChc3IC9fnEBADy
PI81IIIFlCD/FjbFgtEhGPEyvXofoI9kzpZ6E6ehNu7xISxzByIuDb4IZBagri1aM6eEB9
MUF62mKAab+ht9hkTNS0BgVW4a3nZdttYNqcRqTQr2Gn3VQ96RXdwB3Bcwka5ObTS6AF8L
aUe3HDIDfMKOADeTsP7sWSSqCwuoR0+lWfh6b5Y23B1uw3+nefXDfW8fJFFDBBwhwjBCQV
DlI7qJl6EQfdBUuEh68b061HNW6kKxwfiOIfJNCxuUbfh5/BKLFM/i9FJ3rxHKBzQOp+zI
qOQXz4qdabsts1fPyc3pbi7j1BEhZgCtgmH3XPUXiRXEM1dfNi808xRGeapmENFLzjDiB4
mZa6otmGyXRIUOsaZYMwUhG2e1582Es7fnMrAbUNLrsuUViGp30Lb8Tep0/YJflGBsFE0w
rpjbZ0oGvE/6TfdnaN3Gb0n9AYmX2tRAmckdrkZnp3+hSwtiYUBOxycQMCCF8eRfIWBLhO
UAAAdI33ewIN93sCAAAAAHc3NoLXJzYQAAAgEAsTo5Y2iEpAt52qMDXMmqWf7pTExNwRWq
WNtwjlFzUrO2F/D8wKRMqU1lT+GTaAt2/+Nyyt0dZ3j5UMgIXhHmAcuuHlRYzir9MuCmKZ
Xrnq3Tu2RTftbZMbL5MVUXqK0WR57dDqQL5oG5ILdBsT+lpAtOjoLj9Lf593JlMH4MbY6X
cNbxxFChc3IC9fnEBADyPI81IIIFlCD/FjbFgtEhGPEyvXofoI9kzpZ6E6ehNu7xISxzBy
IuDb4IZBagri1aM6eEB9MUF62mKAab+ht9hkTNS0BgVW4a3nZdttYNqcRqTQr2Gn3VQ96R
XdwB3Bcwka5ObTS6AF8LaUe3HDIDfMKOADeTsP7sWSSqCwuoR0+lWfh6b5Y23B1uw3+nef
XDfW8fJFFDBBwhwjBCQVDlI7qJl6EQfdBUuEh68b061HNW6kKxwfiOIfJNCxuUbfh5/BKL
FM/i9FJ3rxHKBzQOp+zIqOQXz4qdabsts1fPyc3pbi7j1BEhZgCtgmH3XPUXiRXEM1dfNi
808xRGeapmENFLzjDiB4mZa6otmGyXRIUOsaZYMwUhG2e1582Es7fnMrAbUNLrsuUViGp3
0Lb8Tep0/YJflGBsFE0wrpjbZ0oGvE/6TfdnaN3Gb0n9AYmX2tRAmckdrkZnp3+hSwtiYU
BOxycQMCCF8eRfIWBLhOUAAAADAQABAAACAGBCi6Eex8yCHzFNkSn4rvoqpnS2jRTuu5N/
vObP/p9Q1Pqz/dR0aN8cFocIspO0hnH+C/97kdj9sAzcWQ8fEZqwEmaO0Z1JZDUaJ6Y2s7
+AEpyZpXAjKd0ApLDS0wLe4FcORmsJVx1gIDlQz/GB7GnpakWlekMVGkP4clWgYQewhzjW
xoImeUrHBiyr+HdkPC4Aao65kGYgdeyO20BublepyjF3/22p9MrwmGXMipfXuEiYZ/Hb8r
+sE8qpL6TrJS8hMWk+kI871h+vV1DFVaxz+j2BPdGo+BcUm1oPcWRgNoyaA4noBsnSPYqJ
UMlGHy9BSX+vP8er1/ra5O3/jDxzqkQubp2Mtm+xtsfai/eClYOHpL3/T3rB64CbVUw9Cr
G+EDExOdw3Zw8mbqkt9v3SiXbvodEn3TRGoWOf4wlPD0YD6FXMsgq1hgSOxPwWKT9Gkojh
QPQlueOScLZA9LdfJ4IzaEj56OYNJiLt/+pw2Mn2/qwPae7Mp8xC/uV35SJ7psykhB9Rly
Crzq/GIE00S+3yR1U2gT3B/MKQasTYvB4y6puQqMNKZwUNyoRcss2DEBUvTAr7lIA41W6y
7MnJ8Xar2Z0TkXMGToXMW47F8N1tOgOCiQ+mB8X5yPze1f9XpcAUrXdeJ0wunwkWZ+uNBc
Bd5kr3SKF+MpMyi/SBAAABAQC/KKjOvy5Y14NS32/MrCoqKtuxytWc12RZUiJSnZ5rTliB
b+rd9BLXQt2PVMeEDKfcwGSB/5cbi/8BaZkwLTw2nHi2bLmCIY/pCMGF+jl6e5H9Ybrt7C
hjKBpHyOYaY9Mf7b0/jcBFIencESB+VYW284GS8Vma+u4hxjsiymK3qllyz9tXwrDQi1Yj
bdhPTmDCHn6uiWgUQZJQ557/ai2iOCwc9zzy6kVkxHH/+M8MTSp4k/ughIH2pXmJ/kJ5SO
CSnFfIdVEiLOdsfLVxMu/TqDgY+pxN+5ZOpsY861JP4Ug0CA6HaZ3AoBa7ckXOhdonkvYL
m1h0WHQWOqqDkWuWAAABAQDeAM6QGfFzh2zXCGsTuxskwTLhvDNnIbNj+nuxRy4AdqlgWI
smxRH+8XXqODnBSeDJsIhLLISRHttLrKdP4qfrvYL+2AXxS92Z843LtDsIwQAjtqpVlZxw
e7V7y30jsYg3Bb5Tx89JHE4kXhS46SW938WgVDzAdoh2DZeDclVKhVx6evWFyJCJHN4mxz
IpiGaWoLn2TC71PlhEZsa4HWdg2IiC+byBc8xK6VMpvxgZFHbr2IyzBWrAUG+1jOxtsHeD
uZxv9fyc+zKkMxg6RN8lG5tNQLz87FqA5FST0mOLDbAhvKqKwXxCguCKp3cBYl/8QBGO7G
/RDNhnhVkjvXmpAAABAQDMXhMDFElCH8N7PQsPOq+AJmrT1BYf2qkLkYwjBkl3pv5lz8fJ
nFBJ/AnIHJ2xYMd17jF5cQOP8XQhyd+EzKTgfGXymEbSs8IXCuk9vcXUCfQjZz+APmcq7G
cLBH04wquFGF/E967FauZTfoYq5Ax0H+dxlnHJnpg49ucyGDqQddmi17lDlnJm504RM7Xv
Y6OUYqB7ckO5cqm9q9w5sA1jQzMvVJPy1NXsBaFKoA0VjT6dlgusXH+5h3p6IlRjy2pNkO
KwFXh8IzDxyhfb6tOA8pWPhBUo/kbW6w0JMkAKqKxW8PboMOZ5nnQBz80nP8SWwQcYMUP+
5hfbPFQuaE7dAAAADGNybUB0ZXN0LmNvbQECAwQFBg==']) {
                        sh '''
                            ssh -o StrictHostKeyChecking=no root@172.17.2.162 whoami
                        '''
                    }
                }
            }
        }
    }
}
