# PentaZen-Gomocup
PentaZen is a gomoku/renju engine supporting gomocup protocol. To run the engine, please download Piskvork gomoku manager from https://gomocup.org/download-gomocup-manager/.
PentaZen��һ��ʹ��gomocupЭ���������/�������档���https://gomocup.org/download-gomocup-manager/����Piskvork������PentaZen��

## Overview
PentaZen engine is written in C. It is compatible with Windows7 and Windows10. It supports freestyle(five or more stones win), standard(exactly five stones win) and renju rules. For freestyle and standard rules, the board size should be 15 * 15 or 20 * 20. For renju rule, the board size should be 15 * 15.
PentaZen��������C���Ա�д�ģ�������Windows7��Windows10���������С�PentaZen֧���޽��֣��޽�������ʤ��������򣨲�֧�ִ��ͽ������������޽��ֹ����£����̴�С������15 * 15��20 * 20��������������̴�Сֻ����15 * 15��

## Algorithm and Performance
PentaZen uses classic searching techniques. The basic algorithm is minimax search with pruning accelerated by hash table and VCF and VCT search. Under gomocup fastgame time limit(5s per move, 120s per match), PentaZen can finish 5-ply to 7-ply pruned minimax search and 10-ply VCT search of one color per move.
PentaZen���ô�ͳ����������������֦�ļ���С�������Լ�VCF��VCT����������С����ʹ����ɢ�б���١���ÿ��5�룬ÿ��120���ʱ���£�PentaZen�о�ÿ�����Ա�֤��ɫ5-7������С�����͵�ɫ10��VCT������
