git �����ܽ�:
1.git reset --hard �汾��    ==>���˵���ǰ�汾��
2.git mv ���ļ��� ���ļ���  ==>�����ļ��� |mv��move����д|
3.git branch -v �鿴�����ж��ٷ�֧
4.git checkout -b ��֧���� �汾��  ==>��������ĳ���汾�ŵķ�֧
5.git checkout ��֧���� ==>�л���֧
6.gitk  ==>���汾��ʷ���湤��
7.git cat-file -p �汾��  ==>��ʾ�汾����������

ʾ��:
$ git cat-file -p 6b734da47b176bd5e8e518df1b17587fa8bf0824
tree 76d4b3d1e2bd50c8cf706fb4ffe3ac30ace8d644
parent 1087f96456c3b2dcb82b03e588cc0d200034b2e4
author zhiqingchun <18519395776@163.com> 1560263371 +0800
committer zhiqingchun <18519395776@163.com> 1560263371 +0800
-----------------------------------------------------------------------------
$ git cat-file -p 76d4b3d1e2bd50c8cf706fb4ffe3ac30ace8d644
100644 blob e91519abba8ad0259772b61c2096dd6bf87e1c36    demo.html
100644 blob ef171b9786a544bf286e135e138353b8b35a8824    vue.js
8.git diff �汾�� ֮ǰ�İ汾��   ==> �汾��֮�����Ƚ�(�޸�����Щ����)
  ������git diff HEAD HEAD~1(HEAD~2)  HEAD�ǵ�ǰ�汾�� HEAD~1����һ���汾��(HEAD~2����һ������һ���汾��)
  ������git diff HEAD HEAD^   ԭ��ͬ��
9.git branch -D ��֧��  ==>ɾ����֧
10.git commit --amend   ==>�޸����һ��commit��������(amend:����;�޶�)
	����֮��,ctrl+c :wq ���沢�˳�
11.git diff --cached  ==>�ݴ�����HEAD�����ļ��Ĳ���
12.git diff  ==>���������ݴ����Ĳ���(�����ļ�)
13.git diff -- �ļ���  ==>���������ݴ���ָ���ļ��Ĳ���
14.git diff ��֧�� ��֧�� -- �ļ���  ==>�Ƚ�������֧��ĳ���ļ��Ĳ���
15.git reset HEAD  ==>(���Ѿ�ʹ��add����ŵ��ݴ�����,�������ݴ����������ļ��ָ���HEAD,���ô�����)
16.git reset HEAD -- �ļ���  ==>�ָ��ݴ��������ļ��ĸ���
17.git checkout -- �ļ���  ==>���������ָ����ݴ���������
18.git rm �ļ���  ==>���ļ���ɾ��,Ȼ��ֱ��commit����
19.git stash  ==>���������޸ĵ�������ʱ�ȴ�����
20.git stash list ==>�鿴stash�б�
21.git stash apply  ==>�ָ�֮ǰ�������ݴ�����������,stash�б�û�����
22.git stash pop  ==>�ָ�֮ǰ�������ݴ�����������,stash�б����
