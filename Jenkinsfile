@Library('piper-lib-os') _

node()
{

stage('Deploy')
	gctsDeploy(
		script: this,
		host:'https://lab-s4bfor.everislab.com:44340',
		client: '210',
		abapCredentialsId: 'ABAPUserPasswordCredentialsId',
		repository: 'vgonzcam-oip_gcts_test_02',
		remoteRepositoryURL: 'https://github.com/vgonzcam/oip_gcts_test_02',
		vSID: 'GIT',
		rollback: true,
		configuration: [VCS_AUTOMATIC_PULL: 'FALSE',VCS_AUTOMATIC_PUSH: 'FALSE',CLIENT_VCS_LOGLVL: 'debug']
	)

}
