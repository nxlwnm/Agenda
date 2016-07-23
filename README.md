# Agenda
实训 School of Software, SYSU

#项目架构
Agenda项目可分为三层,UI层,逻辑层,数据(Data)层
分层如下
AgendaUI
AgendaService
Storage
Meeting，Date，User

#UI层
负责与user交互，将user的操作交付给逻辑层，体现在AgendaUI类

#逻辑层
负责处理user发出的操作，并且对应翻译成对数据层的处理，体现在AgendaService类

#数据层
底层数据的CURD，并且有一个Storage类提供底层数据的操作接口
Storage类采用单例模式，一次只允许一个实例操作底层数据
