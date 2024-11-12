# web2
ups 12.11

case 2:
            subs_range: str = input('Введите диапазон необходимого количества подписок (ex: 2-5, 4-10, 5, 10): ')

            first_int_subs_range, second_int_subs_range = format_range(value=subs_range)

            if second_int_subs_range >= len(accounts_list):
                second_int_subs_range: int = len(accounts_list) - 1

            if first_int_subs_range > second_int_subs_range:
                logger.error('Неверно введен диапазон количества подписок')
                input('\nPress Enter To Exit..')
                exit()

            print()
