
2012-5-10

��ʾ��HTML5��SVG��CANVAS��ϵĹ��ܣ�����SVG PATH���ո���������û����룬��CANVAS��Ϊ��Ч�Ļ�������ͼƬ����ʾ
��Ҫ������
��̬���ɰ������������ߵ�SVG·���ַ���
������ʽ����SVG PATH�ַ���������Ч�Ľ���CANVAS CLIP
�϶�����ת��ͨ��ת����������SVG��CANVAS��ͬ��11

7-4
���IE9+��ʹ��page-������offset�������Ƕ������Ҫѭ������������offsetXY

			if( Sys.ie == null) //For FireFox/Chrome/Safari
			{
				cx = ev.originalEvent.layerX;
				cy = ev.originalEvent.layerY;
			}	
			else //For IE9
			{
				cx = ev.originalEvent.pageX - canvas.offsetLeft;
				cy = ev.originalEvent.pageY - canvas.offsetTop;

			}

���߶�ͳһ��page - canvas��offsetLeft������ʹ��layer���Ƽ���

˳�����Ӽ����򵥵�����Ч��

HTML5ƴͼ��Ϸ����+ͼƬ������

����HTML5���ȣ������˺ܶ���ܣ������ص����CANVAS����Ժ�����SVG���Ҹ��˸о�������������ϣ����ƻ���������SVG�Ľ����Ժ�CANSVAS�Ļ�ͼ���������ܸ��õط��Ӹ��Ե����á�

��ǰ�ô�SVG����һ��ƴͼ��DEMO�����ڸ�ΪSVG��CANVAS������һ�����ڵ�ʱ�䣬��д��������ӣ���CHROME17��FF12�н����˲��ԡ��ȴ�SVG�ٶȿ졣

һֱ����SVG������������ԭ�򣬰���������Ƿ�֧�ֵȵȣ�û�еõ��㷺��Ӧ�á���HTML5�Ŀ���ڣ�SVG�ܹ������Լ�Ӧ�е������˰ɣ�