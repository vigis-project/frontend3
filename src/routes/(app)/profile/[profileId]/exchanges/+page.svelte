<script lang="ts">
    import ActiveExchange from "./ActiveExchange.svelte";

    import type {ExchangeCard } from "$lib/server/types";
    
    const exampleExchangeCard: ExchangeCard = {
    exchange: {
        bookOffer: {
			title: 'Мастер и Маргарита',
			author: 'Михаил Булгаков',
			data: '1967',
			id: 1
		},
        bookRequest: {
			title: 'Война и мир',
			author: 'Лев Толстой',
			data: '1869',
			id: 2
		},
        userOffer: {
            id: 1,
            email: 'offer@example.com',
            username: 'offer_user',
            firstName: 'Иван',
            lastName: 'Иванов',
            secondName: 'Иванович',
            avatar: '/path/to/avatar.jpg',
            rating: 4.8,
            city: 'Москва'
        },
        userRequest: {
            id: 2,
            email: 'request@example.com',
            username: 'request_user',
            firstName: 'Мария',
            lastName: 'Петрова',
            secondName: 'Сергеевна',
            avatar: '/path/to/avatar.jpg',
            rating: 4.6,
            city: 'Санкт-Петербург'
        }
        },
        offerStatus: 'Принято',
        requestStatus: 'Ожидает подтверждения',
        requestNumber: 1111,
        offerNumber: 0,
        
    };

</script>



<ActiveExchange ExchangeCard={exampleExchangeCard}/>

