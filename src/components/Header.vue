<template>
    <div class="header">
        <div class="header-container">
            <div class="header-logo-container">
                <div class="header-logo">
                    <div></div>
                </div>
                <h2>Adilo</h2>
            </div>
            <nav>
                <ul>
                    <li class="nav-link">
                        Project
                    </li>
                    <li class="nav-link">
                        <span>Tools & App</span>
                        
                        <ul class="dropdown">
                            <li>Snapbyte Recorder</li>
                            <li>AudioBounce</li>
                            <li>Sugar Vioce</li>
                        </ul>
                    </li>
                    <li class="nav-link">Channels </li>
                    <li class="nav-link">Contacts</li>
                    <li class="nav-link">Analytics</li>
                    <li class="nav-link">Settings</li>
                </ul>
            </nav>
            <div class="user-profile-container">
                <div class="help">Help</div>
                <div class="user-profile-details">
                    <div class="profile-img-container">
                        <img width="40px" height="40px" src="../assets/danieltwo.jpeg" alt="Profile Picture">
                    </div>
                    <div class="user-details">
                        <div class="user-name">Cody Fisher</div>
                        <div class="user-email">Codyfisher@gmail.com</div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped lang="less">
.header {
    color: black;
    background-color: white;
    height: 80px;
    padding: 0px 2rem;
    display: flex;
    align-items: center;
    border-bottom: 1px solid #0DABD838;

    .header-container {
        display: flex;
        align-items: center;
        justify-content: space-between;
        width: 100%;

        .header-logo-container {
            display: flex;
            align-items: center;
            gap: 1rem;
            cursor: pointer;

            .header-logo {
                background: #FBBD71 0% 0% no-repeat padding-box;
                height: 35px;
                width: 35px;
                border-radius: 10px;
                display: flex;
                align-items: center;
                justify-content: center;

                div {
                    background: white;
                    height: 22px;
                    width: 22px;
                    border-radius: 100%;
                }
            }

            h2 {
                font: normal normal bold 24px/30px Helvetica;
                letter-spacing: 0px;
                color: #21455E;
                opacity: 1;
            }
        }

        nav {
            ul {
                display: flex;
                gap: 2rem;
                list-style-type: none;
                margin: 0;
                padding: 0;
                


                li {
                    text-align: left;
                    font: normal normal medium 18px/27px Poppins;
                    letter-spacing: 0px;
                    color: #707070;
                    opacity: 1;
                    cursor: pointer;
                    position: relative;

                    

                    .dropdown {
                        display: flex;
                        flex-direction: column;
                        position: absolute;
                        background: #FFFFFF 0% 0% no-repeat padding-box;
                        box-shadow: 0px 3px 24px #0000001A;
                        border: 1px solid #E2E5ED;
                        border-radius: 8px;
                        opacity: 1;
                        gap: 0;
                        box-sizing: border-box;
                        text-align: left;
                        display: none;
                        top: 2.5rem;
                        left: -2rem;
                        
                        

                        li {
                            flex: 1;
                            padding: 1rem 2rem;
                            font-weight: 500;
                            white-space: nowrap;
                            color: #21455E;
                            font: normal normal normal 16px/25px Poppins;
                        }

                        li:not(:last-child) {
                            border-bottom: 1px solid #0000001A;
                        }

                        li:hover {
                            color: #0DABD8;
                        }
                    }
                }

                .nav-link::before  {
                    content: ' ';
                    background: #0DABD8;
                    height: .3rem;
                    width: 100%;
                    position: absolute;
                    top: -1.8rem;
                    border-radius: 20px;
                    display: none;
                    
                }

                .nav-link:hover  .dropdown {
                    display: flex;
                }

                .nav-link:hover::before {
                    display: flex;
                }



                li:hover  {
                    color: #21455E;

                }
            }
        }

        .user-profile-container {
            display: flex;
            align-items: center;

            .help {
                font: normal normal medium 18px/27px Poppins;
                    letter-spacing: 0px;
                    color: #21455E;
                    opacity: 1;
                    cursor: pointer;
                    font-weight: 500;
                    padding: 0 1rem;
                    border-right: 1px solid #0DABD838;
            }

            .user-profile-details {
                display: flex;
                gap: 1rem;
                padding-left: 1rem;
                align-items: center;
                justify-content: center;

                .profile-img-container {
                    display: flex;
                    align-items: center;

                    img {
                        border-radius: 100%;
                    }
                }

                .user-details {
                    
                    .user-name {
                        font-size: 15px;
                        font-weight: 600;
                    }

                    .user-email {
                        font-size: 11px;
                        color: #637C8E;
                    }
                }

            }


        }
    }
}




</style>