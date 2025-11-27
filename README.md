<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>IThub College - Система управления учебными проектами</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            background: #0a0a0a;
            color: #e0e0e0;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            padding: 20px;
            background: linear-gradient(135deg, #0a0a0a 0%, #1a1a2e 50%, #16213e 100%);
            min-height: 100vh;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            background: rgba(25, 25, 35, 0.95);
            border-radius: 15px;
            padding: 30px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.5);
            border: 1px solid #333;
        }

        .header {
            text-align: center;
            margin-bottom: 40px;
            padding-bottom: 20px;
            border-bottom: 2px solid #00d4ff;
            background: linear-gradient(135deg, #1a1a2e 0%, #16213e 100%);
            padding: 30px;
            border-radius: 10px;
            border-left: 5px solid #00d4ff;
        }

        .title {
            font-size: 2.5em;
            background: linear-gradient(45deg, #00d4ff, #0099cc);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            margin-bottom: 10px;
            font-weight: bold;
        }

        .subtitle {
            font-size: 1.2em;
            color: #88ccff;
            opacity: 0.9;
        }

        .section {
            margin-bottom: 35px;
            padding: 25px;
            background: rgba(40, 40, 55, 0.6);
            border-radius: 10px;
            border-left: 4px solid #00d4ff;
            transition: transform 0.3s ease;
        }

        .section:hover {
            transform: translateX(5px);
            background: rgba(50, 50, 65, 0.7);
        }

        .section-title {
            font-size: 1.5em;
            color: #00d4ff;
            margin-bottom: 15px;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .section-title::before {
            content: "▶";
            font-size: 0.8em;
            color: #00d4ff;
        }

        .feature-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 15px;
            margin-top: 15px;
        }

        .feature-card {
            background: rgba(60, 60, 80, 0.4);
            padding: 15px;
            border-radius: 8px;
            border: 1px solid #444;
            transition: all 0.3s ease;
        }

        .feature-card:hover {
            border-color: #00d4ff;
            transform: translateY(-2px);
            box-shadow: 0 5px 15px rgba(0, 212, 255, 0.2);
        }

        .role-card {
            background: rgba(70, 70, 90, 0.4);
            padding: 20px;
            border-radius: 8px;
            margin-bottom: 15px;
            border-left: 3px solid #0099cc;
        }

        .role-title {
            color: #00d4ff;
            font-weight: bold;
            margin-bottom: 8px;
            font-size: 1.1em;
        }

        .tech-badge {
            display: inline-block;
            background: linear-gradient(45deg, #0099cc, #0077aa);
            color: white;
            padding: 5px 12px;
            border-radius: 20px;
            font-size: 0.9em;
            margin: 5px 5px 5px 0;
            border: 1px solid #00aaff;
        }

        .contact-link {
            color: #00d4ff;
            text-decoration: none;
            transition: color 0.3s ease;
            display: inline-flex;
            align-items: center;
            gap: 5px;
        }

        .contact-link:hover {
            color: #88eeff;
            text-decoration: underline;
        }

        .structure {
            background: rgba(30, 30, 45, 0.8);
            padding: 20px;
            border-radius: 8px;
            font-family: 'Courier New', monospace;
            border: 1px solid #444;
            margin-top: 10px;
        }

        .file-tree {
            color: #88ccff;
            line-height: 1.8;
        }

        .file-tree div {
            margin-left: 20px;
        }

        .status-bar {
            display: flex;
            gap: 20px;
            margin-top: 20px;
            padding-top: 20px;
            border-top: 1px solid #444;
            flex-wrap: wrap;
        }

        .status-item {
            background: rgba(60, 60, 80, 0.6);
            padding: 10px 15px;
            border-radius: 8px;
            border: 1px solid #555;
        }

        .emoji {
            font-size: 1.2em;
            margin-right: 8px;
        }

        .highlight {
            color: #00d4ff;
            font-weight: bold;
        }

        @media (max-width: 768px) {
            .container {
                padding: 15px;
            }
            
            .title {
                font-size: 2em;
            }
            
            .feature-grid {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <!-- Заголовок -->
        <div class="header">
            <h1 class="title">🎓 IThub College - Система управления учебными проектами</h1>
            <p class="subtitle">Профессиональная платформа для организации студенческих проектов</p>
        </div>

        <!-- Описание проекта -->
        <div class="section">
            <h2 class="section-title">🤐 Описание проекта</h2>
            <p>Веб-платформа для управления студенческими проектами в колледже IThub. Система позволяет отслеживать прогресс проектов, назначать задачи и координировать работу между студентами и преподавателями.</p>
            
            <div class="feature-grid">
                <div class="feature-card">
                    <strong>Для кого предназначен проект:</strong>
                    <ul style="margin-left: 20px; margin-top: 10px;">
                        <li>Студенты IThub - разработчики, дизайнеры, менеджеры</li>
                        <li>Преподаватели и кураторы - контроль выполнения работ</li>
                        <li>Администрация колледжа - отслеживание проектной деятельности</li>
                    </ul>
                </div>
                
                <div class="feature-card">
                    <strong>Основные функции:</strong>
                    <ul style="margin-left: 20px; margin-top: 10px;">
                        <li>Создание и ведение учебных проектов</li>
                        <li>Назначение ролей в команде (менеджер, разработчик, дизайнер)</li>
                        <li>Контроль сроков и дедлайнов</li>
                        <li>Система отчетности и отслеживания прогресса</li>
                        <li>Хранение всей проектной документации</li>
                    </ul>
                </div>
            </div>
        </div>

        <!-- Установка и запуск -->
        <div class="section">
            <h2 class="section-title">🕸️ Установка и запуск</h2>
            
            <div class="feature-card">
                <strong>Что потребуется:</strong>
                <div style="margin-top: 10px;">
                    <span class="tech-badge">Компьютер с Windows/Mac/Linux</span>
                    <span class="tech-badge">Браузер (Chrome, Firefox, Edge)</span>
                    <span class="tech-badge">Доступ в интернет</span>
                </div>
            </div>
            
            <div class="feature-card" style="margin-top: 15px;">
                <strong>Как начать пользоваться:</strong>
                <ol style="margin-left: 20px; margin-top: 10px;">
                    <li>Перейдите на сайт системы (адрес будет добавлен после развертывания)</li>
                    <li>Зарегистрируйтесь используя вашу учебную почту IThub</li>
                    <li>Создайте первый проект - заполните основную информацию</li>
                    <li>Пригласите团队成员 - добавьте участников по их email</li>
                    <li>Начните работу - создавайте задачи и отслеживайте прогресс</li>
                </ol>
            </div>
        </div>

        <!-- Примеры использования -->
        <div class="section">
            <h2 class="section-title">👨🏿‍🦱 Примеры использования</h2>
            
            <div class="feature-grid">
                <div class="feature-card">
                    <strong>Для менеджера проекта:</strong>
                    <p>Проект: "Разработка интернет-магазина"</p>
                    <p><strong>Команда:</strong></p>
                    <ul style="margin-left: 20px;">
                        <li>Менеджер: Иванов Алексей</li>
                        <li>Frontend-разработчик: Петрова Мария</li>
                        <li>Backend-разработчик: Сидоров Дмитрий</li>
                        <li>Дизайнер: Кузнецова Анна</li>
                    </ul>
                    <p><strong>Этапы работы:</strong></p>
                    <ul style="margin-left: 20px;">
                        <li>Анализ требований</li>
                        <li>Прототипирование (в процессе)</li>
                        <li>Разработка (ожидание)</li>
                        <li>Тестирование (ожидание)</li>
                    </ul>
                </div>
                
                <div class="feature-card">
                    <strong>Для разработчика:</strong>
                    <ul style="margin-left: 20px;">
                        <li>Просмотр назначенных задач</li>
                        <li>Отметка о выполнении этапов</li>
                        <li>Загрузка готового кода</li>
                        <li>Коммуникация с командой</li>
                    </ul>
                </div>
            </div>
        </div>

        <!-- Структура репозитория -->
        <div class="section">
            <h2 class="section-title">📁 Структура репозитория</h2>
            <div class="structure">
                <div class="file-tree">
                    IThub-Project-Management/<br>
                    <div>
                        ├── 📄 README.md &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# Главная документация<br>
                        ├── 📁 docs/ &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# Документация проекта<br>
                        ├── 📁 presentations/ &nbsp;# Презентации и отчеты<br>
                        ├── 📁 research/ &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# Исследования и аналитика<br>
                        └── 📁 assets/ &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# Изображения и ресурсы
                    </div>
                </div>
            </div>
        </div>

        <!-- Технические требования -->
        <div class="section">
            <h2 class="section-title">⚙️ Технические требования</h2>
            
            <div class="feature-grid">
                <div class="feature-card">
                    <strong>Для использования системы:</strong>
                    <div style="margin-top: 10px;">
                        <span class="tech-badge">Браузер: Chrome 90+</span>
                        <span class="tech-badge">Firefox 88+</span>
                        <span class="tech-badge">Safari 14+</span>
                        <span class="tech-badge">Стабильный интернет</span>
                        <span class="tech-badge">ПК/Ноутбук/Планшет</span>
                    </div>
                </div>
                
                <div class="feature-card">
                    <strong>Для разработки (если потребуется):</strong>
                    <div style="margin-top: 10px;">
                        <span class="tech-badge">JavaScript</span>
                        <span class="tech-badge">React</span>
                        <span class="tech-badge">MongoDB</span>
                        <span class="tech-badge">Node.js</span>
                    </div>
                </div>
            </div>
        </div>

        <!-- Авторы и участники -->
        <div class="section">
            <h2 class="section-title">👥 Авторы и участники</h2>
            <p><strong>Команда проекта:</strong></p>
            
            <div class="role-card">
                <div class="role-title">🎯 Иванов Алексей - Project Manager</div>
                <ul style="margin-left: 20px;">
                    <li>Управление проектом</li>
                    <li>Документация и отчетность</li>
                    <li>Коммуникация с заказчиком</li>
                </ul>
            </div>
            
            <div class="role-card">
                <div class="role-title">💻 Петрова Мария - Frontend Developer</div>
                <ul style="margin-left: 20px;">
                    <li>Разработка пользовательского интерфейса</li>
                    <li>Верстка и визуальное оформление</li>
                </ul>
            </div>
            
            <div class="role-card">
                <div class="role-title">⚙️ Сидоров Дмитрий - Backend Developer</div>
                <ul style="margin-left: 20px;">
                    <li>Серверная часть приложения</li>
                    <li>База данных и API</li>
                </ul>
            </div>
            
            <div class="role-card">
                <div class="role-title">🎨 Кузнецова Анна - UI/UX Designer</div>
                <ul style="margin-left: 20px;">
                    <li>Дизайн интерфейса</li>
                    <li>Прототипирование и用户体验</li>
                </ul>
            </div>
        </div>

        <!-- Контактная информация -->
        <div class="section">
            <h2 class="section-title">📞 Контактная информация</h2>
            
            <div class="feature-grid">
                <div class="feature-card">
                    <strong>По вопросам сотрудничества:</strong>
                    <div style="margin-top: 10px;">
                        <p><a href="mailto:projects@ithub.ru" class="contact-link">📧 Email: projects@ithub.ru</a></p>
                        <p><a href="https://t.me/IThubProjects" class="contact-link">📱 Telegram: @IThubProjects</a></p>
                        <p><a href="https://github.com/IThub-Student" class="contact-link">💻 GitHub: github.com/IThub-Student</a></p>
                    </div>
                </div>
                
                <div class="feature-card">
                    <strong>Техническая поддержка:</strong>
                    <div style="margin-top: 10px;">
                        <p><a href="mailto:support@ithub.ru" class="contact-link">🔧 Email: support@ithub.ru</a></p>
                        <p class="contact-link">💬 Чат в системе управления проектами</p>
                    </div>
                </div>
            </div>
        </div>

        <!-- Статус -->
        <div class="status-bar">
            <div class="status-item">
                <span class="emoji">📊</span> <strong>Статус проекта:</strong> <span class="highlight">В разработке</span>
            </div>
            <div class="status-item">
                <span class="emoji">🎯</span> <strong>Версия:</strong> <span class="highlight">1.0.0</span>
            </div>
            <div class="status-item">
                <span class="emoji">📅</span> <strong>Последнее обновление:</strong> <span class="highlight">Декабрь 2024</span>
            </div>
        </div>

        <div style="text-align: center; margin-top: 30px; padding-top: 20px; border-top: 1px solid #444; color: #888;">
            <em>Проект разработан в рамках учебной программы колледжа IThub</em>
        </div>
    </div>
</body>
</html>
