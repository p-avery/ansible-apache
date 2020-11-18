node {
    stage('MyStage') {
        ansibleTower(
            towerServer: 'Tower',
            templateType: 'job',
            jobTemplate: 'Install_Apache',
            limit: 'dev',
            extraVars: '''---
apache_test_message:  "Jenkins did this!!"''',
            importTowerLogs: true,
            removeColor: false,
            verbose: true,
            async: false
        )
    }
}
