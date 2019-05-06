# PentaZen-Gomocup
PentaZen is a gomoku/renju engine supporting Gomocup protocol. Please compile first and download Piskvork gomoku manager from https://gomocup.org/download-gomocup-manager to run it.

## Overview
PentaZen engine is written in C. It is compatible with Windows7 and Windows10. It supports freestyle(five or more stones win), standard(exactly five stones win) and renju rules. For freestyle and standard rules, the board size should be 15 * 15 or 20 * 20. For renju rule, the board size should be 15 * 15. In Gomocup 2019, PentaZen ranks 19th in freestyle league and 16th in fastgame league.

## Algorithm and Performance
PentaZen uses classic searching techniques. The basic algorithm is minimax search with pruning accelerated by hash table. Under Gomocup fastgame time limit(5s per move, 120s per match), PentaZen can finish 30-ply VCF search, 20-ply VCT search and 10-ply to 14-ply pruned minimax search per step.

# PentaZen-Gomocup
PentaZen��֧��GomocupЭ���������/�������档�ڹ��������֮����Piskvork����exe�ļ��������С�Piskvork���ص�ַ��https://gomocup.org/download-gomocup-manager

## ���
PentaZen��������C���Ա�д�ģ�������Windows7��Windows10���������С�PentaZen֧���޽��֣��޽�������ʤ��������򣨲�֧�ִ��ͽ������������޽��ֹ����£����̴�С������15 * 15��20 * 20��������������̴�Сֻ����15 * 15����2019��Gomocup����������AI�������У�PentaZen������������19λ��������������16λ��

## �㷨����
PentaZen���ô�ͳ����������������֦�ļ���С������ɢ�б���١���ÿ��5�룬ÿ��120���ʱ���£�PentaZenÿ�����������30��VCF��ɱ��20��VCT��ɱ��10-14������֦�ļ���С������
