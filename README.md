

#��������DEMO

    1���ڰ�׿�豸�а�װPeergine�м��,��װ��Ϊ��pgPlugin_XXXXX.apk��
	
	2��Ȼ���ڰ�׿�豸�а�װDemo���򣬰�װ��ΪDemoApp/Demo_XXXXXX.apk��
	
	3���ظ�����1�Ͳ���2,��װ��������׿�豸��
	
	4�����ݽ�������ʾ�����а�׿�豸��������ͬ����ID������һ̨����Ϊ��ϯ��Chairman��������Ϊ����ϯ��
	
	5���鿴��Ƶ����Ч����

	
#����ʹ�û���ģ�鿪��APP
	
	1��ʹ��AndroidStudio�������̡�
	
	2���� pgLibConference ��Ϊģ��(Module)�����㴴���Ĺ��̡�
	
	3���� pgPluginLib ��Ϊģ��(Module)�����㴴���Ĺ��̡�

	4������� Module ����Ӷ� pgLibConference pgPluginLib ������ (��Android Studio��ѡ������ app �� Module ��
����˵�Build->Edit Libraries and Dependencies,�ڵ����ĶԻ������Ͻ��и���ɫ��+�ţ����ѡ��Module Dependency).
	
	5�����Խ�Demo������Ĺ��̣��ο�
	private pgLibConference.OnEventListener m_OnEvent = new pgLibConference.OnEventListener() {
		@Override
		public void event(String sAct, String sData, final String sPeer) {
		}
	}��
	�����¼������������ǵĿ��NodeJsһ�������¼������ġ�
	
	
v1.0.5
1.�����Ƶ�ⲿ�ɼ��ӿڲ���VideoInExternal
2.��Ƶ���Ƕȵ���������
3.���API��������������չ��Ϣ
4.����¼�PeerSync��ʾ������Զ˽���ͨ������������MessageSend����ͨ�š�
5.����¼�PeerOffline��ʾ�Զ��Ѿ����ߡ�
6.����¼�VideoLost����������Ƶ�Ѿ���ʧ
7.�ڲ���ӳ�Ա�˶���ϯ�˵��������Լӿ콫�����쳣�����Ӧ�ó���
8.�ڲ������Ƶ����ʱ���������Լ���쳣����ʱ�Զ˲��ܼ�ʱ��ȡ��Ƶ��ʧ����Ϣ��
�����������Ż����޸�������BUG��

updata 2016/11/17 v1.0.6
 * �����Ƶ��ץ�ĺ�¼�ƹ���
 * ����һ����ʱ��� ��ִ��MemberAdd MemberDel Leave ������ ���45����û���˳��ͼ������   ���Ͳ���TimeOut �Ļص�    sData ��������   sPeer�ǲ���
 �������CallSend ���ܱȽ�MessageSend�����CallSend�Ļ�ִ
 CallSend���������һ�������Զ���
 CallSend�ص��¼���sData �Ǵ������ 0������ ��sPeer��CallSend�����һ������